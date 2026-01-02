
<div>

<span>

<span>

<canvas>

</canvas>

<canvas>

</canvas>

<script>
document.addEventListener('DOMContentLoaded', () => {
            // キャンバス要素の取得
            const groundCanvas = document.getElementById('groundCanvas');
            const snowCanvas = document.getElementById('snowCanvas');
            const snowCtx = snowCanvas.getContext('2d');
            const groundCtx = groundCanvas.getContext('2d');

            // 雪と地面の雪の配列
            let leaves = [];
            let groundLeaves = [];

            // スクロール位置を取得する関数
            const getScrollProgress = () => {
              const scrollHeight = document.documentElement.scrollHeight - window.innerHeight;
              const currentScroll = window.scrollY;
              return Math.min(currentScroll / scrollHeight, 1);
            };

            // スクロール位置に基づいて雪の透明度を決定
            const getSnowColor = (scrollProgress = null) => {
              const progress = scrollProgress !== null ? scrollProgress : getScrollProgress();
              
              // 雪は白で、透明度のみ変化
              const opacity = 0.6 + Math.random() * 0.3;
              return `rgba(180, 220, 255, ${opacity})`;
            };

            // キャンバスのリサイズ処理
            const resizeCanvas = () => {
              const fullHeight = window.innerHeight;
              snowCanvas.width = window.innerWidth;
              snowCanvas.height = fullHeight;
              groundCanvas.width = window.innerWidth;
              groundCanvas.height = fullHeight;
            };

            // 初期化
            resizeCanvas();
            window.addEventListener('resize', resizeCanvas);

            // 雪の生成（画面中央を避ける）
            const createSnow = (x = null, y = null) => {
              let snowX;

              if (x !== null) {
                snowX = x;
              } else {
                // 画面中央を避けて左右どちらかに生成
                const centerZone = snowCanvas.width * 0.6; // 中央60%を避ける
                const leftZone = (snowCanvas.width - centerZone) / 2;
                const rightZoneStart = leftZone + centerZone;

                if (Math.random() < 0.5) {
                  // 左側に生成
                  snowX = Math.random() * leftZone;
                } else {
                  // 右側に生成
                  snowX = rightZoneStart + Math.random() * leftZone;
                }
              }

              const snowY = y !== null ? y : -30;
              const size = 5 + Math.random() * 10;
              const speed = 0.5 + Math.random() * 1.5;
              const swaySpeed = 0.02 + Math.random() * 0.03;
              const swayAmount = 30 + Math.random() * 40;
              const rotation = Math.random() * Math.PI * 2;
              const rotationSpeed = (Math.random() - 0.5) * 0.04;
              const color = getSnowColor();

              leaves.push({
                x: snowX,
                y: snowY,
                initialX: snowX,
                size,
                speed,
                swaySpeed,
                swayAmount,
                swayOffset: Math.random() * Math.PI * 2,
                rotation,
                rotationSpeed,
                color,
                type: Math.random() // 雪の形のバリエーション用
              });
            };

            // 地面に落ちた雪の追加
            const addGroundSnow = (x, y, color, size, type) => {
              groundLeaves.push({
                x,
                y,
                color,
                size,
                rotation: Math.random() * Math.PI * 2,
                opacity: 0.5,
                fadeSpeed: 0.01 + Math.random() * 0.02, // 徐々に透明になる速度
                type
              });

              if (groundLeaves.length > 50) {
                groundLeaves.shift();
              }
            };

            // 自然な雪の結晶を描画
            const drawSnow = (ctx, x, y, size, rotation, color, type) => {
              ctx.save();
              ctx.translate(x, y);
              ctx.rotate(rotation);

              const branches = 6; // 雪の結晶は6方向が基本
              const opacity = parseFloat(color.match(/[\d.]+(?=\))/)[0]);

              ctx.strokeStyle = color;
              ctx.fillStyle = color;
              ctx.lineWidth = size * 0.08;
              ctx.lineCap = 'round';

              if (type < 0.3) {
                // タイプ1: シンプルな六角形の雪
                ctx.beginPath();
                for (let i = 0; i < branches; i++) {
                  const angle = (Math.PI * 2 / branches) * i;
                  const x1 = Math.cos(angle) * size * 0.5;
                  const y1 = Math.sin(angle) * size * 0.5;
                  
                  if (i === 0) ctx.moveTo(x1, y1);
                  else ctx.lineTo(x1, y1);
                }
                ctx.closePath();
                ctx.stroke();
                
                // 中心の点
                ctx.beginPath();
                ctx.arc(0, 0, size * 0.15, 0, Math.PI * 2);
                ctx.fill();
              } else if (type < 0.7) {
                // タイプ2: 枝分かれのある雪の結晶
                for (let i = 0; i < branches; i++) {
                  const angle = (Math.PI * 2 / branches) * i;
                  
                  ctx.save();
                  ctx.rotate(angle);
                  
                  // 主軸
                  ctx.beginPath();
                  ctx.moveTo(0, 0);
                  ctx.lineTo(0, -size * 0.6);
                  ctx.stroke();
                  
                  // 側枝
                  const branchCount = 2;
                  for (let j = 1; j <= branchCount; j++) {
                    const pos = -size * 0.2 * j;
                    const branchLen = size * 0.15 * (branchCount - j + 1) / branchCount;
                    
                    ctx.beginPath();
                    ctx.moveTo(0, pos);
                    ctx.lineTo(-branchLen * Math.cos(Math.PI / 6), pos - branchLen * Math.sin(Math.PI / 6));
                    ctx.moveTo(0, pos);
                    ctx.lineTo(branchLen * Math.cos(Math.PI / 6), pos - branchLen * Math.sin(Math.PI / 6));
                    ctx.stroke();
                  }
                  
                  ctx.restore();
                }
                
                // 中心部
                ctx.beginPath();
                ctx.arc(0, 0, size * 0.1, 0, Math.PI * 2);
                ctx.fill();
              } else {
                // タイプ3: 複雑な樹枝状雪結晶
                for (let i = 0; i < branches; i++) {
                  const angle = (Math.PI * 2 / branches) * i;
                  
                  ctx.save();
                  ctx.rotate(angle);
                  
                  // 主軸
                  ctx.beginPath();
                  ctx.moveTo(0, 0);
                  ctx.lineTo(0, -size * 0.7);
                  ctx.stroke();
                  
                  // 複雑な側枝パターン
                  for (let j = 1; j <= 3; j++) {
                    const pos = -size * 0.18 * j;
                    const branchLen = size * (0.25 - j * 0.05);
                    
                    // 主側枝
                    for (let side of [-1, 1]) {
                      ctx.beginPath();
                      ctx.moveTo(0, pos);
                      ctx.lineTo(
                        side * branchLen * Math.cos(Math.PI / 6),
                        pos - branchLen * Math.sin(Math.PI / 6)
                      );
                      ctx.stroke();
                      
                      // 副側枝
                      const subLen = branchLen * 0.4;
                      ctx.beginPath();
                      ctx.moveTo(
                        side * branchLen * 0.6 * Math.cos(Math.PI / 6),
                        pos - branchLen * 0.6 * Math.sin(Math.PI / 6)
                      );
                      ctx.lineTo(
                        side * (branchLen * 0.6 * Math.cos(Math.PI / 6) + subLen * Math.cos(Math.PI / 4)),
                        pos - (branchLen * 0.6 * Math.sin(Math.PI / 6) + subLen * Math.sin(Math.PI / 4))
                      );
                      ctx.stroke();
                    }
                  }
                  
                  // 先端の装飾
                  ctx.beginPath();
                  ctx.arc(0, -size * 0.7, size * 0.08, 0, Math.PI * 2);
                  ctx.fill();
                  
                  ctx.restore();
                }
                
                // 中心の六角形
                ctx.beginPath();
                for (let i = 0; i < 6; i++) {
                  const angle = (Math.PI * 2 / 6) * i;
                  const x1 = Math.cos(angle) * size * 0.12;
                  const y1 = Math.sin(angle) * size * 0.12;
                  if (i === 0) ctx.moveTo(x1, y1);
                  else ctx.lineTo(x1, y1);
                }
                ctx.closePath();
                ctx.fill();
              }

              ctx.restore();
            };

            // 雪の更新と描画
            const updateLeaves = () => {
              snowCtx.clearRect(0, 0, snowCanvas.width, snowCanvas.height);

              // 新しい雪を生成
              if (Math.random() < 0.06 && leaves.length < 40) {
                createSnow();
              }

              // 既存の雪を更新
              for (let i = leaves.length - 1; i >= 0; i--) {
                const snow = leaves[i];

                // 落下と横揺れ
                snow.y += snow.speed;
                snow.swayOffset += snow.swaySpeed;
                snow.x = snow.initialX + Math.sin(snow.swayOffset) * snow.swayAmount;

                // 回転
                snow.rotation += snow.rotationSpeed;

                // 地面に到達したら
                if (snow.y >= snowCanvas.height * 0.95) {
                  addGroundSnow(snow.x, snowCanvas.height * 0.95, snow.color, snow.size, snow.type);
                  leaves.splice(i, 1);
                  continue;
                }

                // 雪を描画
                drawSnow(snowCtx, snow.x, snow.y, snow.size, snow.rotation, snow.color, snow.type);
              }
            };

            // 地面の雪の更新と描画
            const updateGroundLeaves = () => {
              groundCtx.clearRect(0, 0, groundCanvas.width, groundCanvas.height);

              for (let i = groundLeaves.length - 1; i >= 0; i--) {
                const snow = groundLeaves[i];
                snow.opacity -= snow.fadeSpeed;

                if (snow.opacity <= 0) {
                  groundLeaves.splice(i, 1);
                  continue;
                }

                // 地面の雪は透明度を上書き
                const colorWithOpacity = `rgba(255, 255, 255, ${snow.opacity})`;
                drawSnow(groundCtx, snow.x, snow.y, snow.size * 0.8, snow.rotation, colorWithOpacity, snow.type);
              }
            };

            // クリックイベントの処理
            document.addEventListener('click', (e) => {
              const x = e.clientX;
              const y = e.clientY;

              // クリック位置に雪を生成
              for (let i = 0; i < 3; i++) {
                setTimeout(() => {
                  createSnow(x + (Math.random() - 0.5) * 50, y);
                }, i * 100);
              }
            });

            // アニメーションループ
            const animate = () => {
              updateLeaves();
              updateGroundLeaves();
              requestAnimationFrame(animate);
            };

            animate();
          });

        
</script>

### **コンテスト情報**

<section>

<ul>

<li>
コンテスト時間: 100 分
</li>

<li>
レーティング更新対象: 0 - 
<span>
1999
</span>

</li>

</ul>

</section>

---

### **コンテスト概要**

<section>

<div>

<img src="https://img.atcoder.jp/abc372/uv_abc_banner.png">

</img>

<p>

<span>
当コンテストは、<a href="https://www.uniquevision.co.jp/">
<font color="#D6124B">ユニークビジョン株式会社</font>
</a>
<img src="https://img.atcoder.jp/abc346/icon.png">

</img>
が主催するプログラミングコンテストです。
      
</span>

</p>

<p>

</p>

<div>
<a href="https://atcoder.jp/contests/abc437#office-event">ABC437参加者限定イベント
        
<svg>

<polyline>

</polyline>

</svg>
</a><a href="https://atcoder.jp/contests/abc437#campaign">Amazonギフトカードが当たる！UV賞キャンペーン
        
<svg>

<polyline>

</polyline>

</svg>
</a><a href="https://jobs.atcoder.jp/offers/list?f.CompanyScreenName=uniquevision">AtCoderJobs
              
<svg>

<path>

</path>

<polyline>

</polyline>

<line>

</line>

</svg>
</a>
</div>

<p>

</p>

</div>

</section>

---

### **なぜユニークビジョンがコンテストを実施するのか**

<section>

<p>
このコンテスト開催を通じて、技術が好きなAtCoderユーザーの皆様にユニークビジョンのことを知っていただき、是非とも一緒に技術で世の中を変えていく仲間となっていただきたいと思っています。
  
</p>

<p>
私たちは企業とファンをつなぐSNSマーケティングツールを開発・提供しているテクノロジーカンパニーです。
  
</p>

<p>
SNSは情報の展開が早く影響力の高いメディアであるため、当社のクライアントである大手企業がSNSで実施するキャンペーンは品質やスピードの面でシビアなものがほとんどです。こうした高負荷・高難易度な開発において、皆様には競技プログラミングで培われた「
<b>
決められた時間内でいかに問題を解決していくか
</b>
」という能力を活かし、ユニークビジョンでご活躍いただきたいと思っています。
  
</p>

<p>
実際に、社内にも
    
<b>

<span>
橙色コーダー1名
</span>
、
<span>
黄色コーダー1名
</span>
、
<span>
青色コーダー7名 
</span>
、
      
<span>
水色コーダー6名
</span>
、
<span>
緑色コーダー3名
</span>

</b>
、その他数名の競技プログラマーが在籍しており、競技プログラマーの皆様とは高い親和性を感じております！
  
</p>

</section>

---

### **ユニークビジョンのサービス**

<p>
SNSマーケティングをより効果的に運営するための「
<b>
Belugaシリーズ
</b>
」を開発・運用しています。ソーシャルメディアを活用した、幅広いマーケティング施策で企業の
<b>
ブランド体験の創出
</b>
に貢献しています。
  
</p>

<div>

<img src="https://img.atcoder.jp/abc437/27b1ad9a5167126faf15bec1adebaa5c.png">

</img>

</div>

<section>

<p>
<a href="https://www.uniquevision.co.jp/service/beluga-campaign/">
<img src="https://img.atcoder.jp/abc437/a0ac12bf693369e5412e182cd4313753.png">

</img>
</a>
</p>

<p>
X・LINE・Instagramにて自動返信やインスタントウィン（その場で抽選、当落の確認）キャンペーンを提供。スピーディで品質の高いキャンペーンを実現します。
  
</p>

<p>
<a href="https://www.uniquevision.co.jp/service/beluga/">
<img src="https://img.atcoder.jp/abc437/a4ab8fa08e982bea763078ccc98a7899.png">

</img>
</a>
</p>

<p>
X（旧Twitter）・Facebook・Instagramのアカウントを一元管理できるツールとして、企業のSNS運用をサポートします。
  
</p>

<p>
<a href="https://www.uniquevision.co.jp/service/beluga-crm">
<img src="https://img.atcoder.jp/abc437/d1d5fe04379a31ccff5eed0f5ffb86d2.png">

</img>
</a>
</p>

<p>
BelugaキャンペーンやBelugaスタジオで取得できるデータを蓄積し、分析・活用できるプラットフォームとして提供。キャンペーンの精度を向上させることで、ロイヤル顧客の醸成につなげます。
  
</p>

<p>
上記以外にも、様々なBelugaシリーズ製品を開発・運用しています。
</p>

</section>

#### **▮導入事例▮**

<section>

<p>
Belugaシリーズは2011年のリリース以来、大手企業を中心にのべ
<span>
500
</span>

<span>
社
</span>
の企業に導入され、約
<span>
5000
</span>

<span>
件
</span>
の施策に利用していただいております。
  
</p>

<p>
▼例えば…
  
</p>

<ul>

<li>

<p>
<a href="https://www.uniquevision.co.jp/case/belugacampaignforx-lawson-karaagekun39th">𝕏：ローソン×絵文字投稿×自動返信施策　
<span>
★トレンド入り★
</span>

<svg>

<path>

</path>

<polyline>

</polyline>

<line>

</line>

</svg>
</a>
</p>

</li>

<li>

<p>
<a href="https://www.uniquevision.co.jp/case/belugacampaignforx-mixi-aiwakatter">𝕏：MIXI×AI×画像合成施策　
<span>
★トレンド入り★
</span>

<svg>

<path>

</path>

<polyline>

</polyline>

<line>

</line>

</svg>
</a>
</p>

</li>

<li>

<p>
<a href="https://www.uniquevision.co.jp/case/asahiinryo-mituya-christmas">LINE：アサヒ飲料×購入レシートで賞品応募施策
          
<svg>

<path>

</path>

<polyline>

</polyline>

<line>

</line>

</svg>
</a>
</p>

</li>

<li>

<p>
<a href="https://www.uniquevision.co.jp/case/belugacampaignforinstagram-pubgmobile-frieren">Instagram：PUBG MOBILE×アニメコラボ×自動抽選施策
          
<svg>

<path>

</path>

<polyline>

</polyline>

<line>

</line>

</svg>
</a>
</p>

</li>

</ul>

<p>
その他の事例は<a href="https://www.uniquevision.co.jp/case">こちら</a>よりご覧ください！
  
</p>

</section>

---

### **技術スタック**

<section>

#### **主要開発言語**

<ul>

<li>

<span>
Rust
</span>

</li>

</ul>

#### **開発言語**

<ul>

<li>
TypeScript、SQL、Ruby、Python3
</li>

</ul>

#### **フレームワーク**

<ul>

<li>
Vue.js、axum、actix-web、Ruby on Rails、Node.js、Sinatra
            
</li>

</ul>

#### **データベース**

<ul>

<li>
PostgreSQL、DynamoDB
</li>

</ul>

#### **環境**

<ul>

<li>
nginx、Redis、Linux、Amazon Web Service、Google Cloud、BigQuery
            
</li>

</ul>

#### **プロジェクト管理**

<ul>

<li>
Git
</li>

</ul>

</section>

---

### **社内競技プログラミング部員のメッセージ**

<section>

<p>
数年前まで社内に競技プログラマーはほぼいなかったのですが、年々増え続け、今では15名以上の競技プログラマーが在籍しています。有志で競技プログラミング部を作り、出場したいコンテストの仲間を募ったり、問題の振り返りをしたりという活動をしています！
          
</p>

<p>
競プロユーザーがいなかった時代もあったので、社員同士でチーム戦のコンテストに出たときはとても嬉しかったです。
            実際の案件でも、再帰関数・トポロジカル順序など競技プログラミングの知識を活かしてスピード感のある実装を叶えられている業務もあります。
          
</p>

<p>
共通の話題があるので打ち解けるのも早いですし、AtCoderさんの本社が近いことも密かに嬉しいポイントです(笑)

気になった方は是非、UV Study（勉強会）などで遊びに来てください！
          
</p>

</section>

<div>

<img src="https://img.atcoder.jp/abc334/Competitive_programming_club.png">

</img>

</div>

---

### **社内AtCoderユーザーからのメッセージ**

<section>

<p>
ユニークビジョンでは担当業務に関わらずスピード感を持った開発と高いパフォーマンスや可用性が求められており、その実現のためにエンジニア主導で新しい技術の導入や開発体験を高めるための改善の検討を行うなど、改善意欲のあるエンジニアが力を発揮しやすい職場となっています。
          
</p>

<p>
また、主要サービスであるBelugaキャンペーンは柔軟で表現能力が高く未知のキャンペーンでも多くの場合追加開発なしで行うことが出来るようになっています。一方で、その柔軟さ故に案件実現の可否を判断するためには深い業務知識と問題の本質を見抜く能力、パフォーマンス的に問題が無いかを判断する計算量などの知識が必要で簡単ではありません。こういった業務は通常のWebアプリケーション開発にはない面白さがあり、競技プログラミングで培った知識や思考力を活かしていただけるのではないかと期待しています。
          
</p>

<p>
向上心の高いエンジニアが多く、競技プログラミングをはじめ様々な技術分野について社内で議論することが出来ます。少しでもご興味を持たれた方は是非、オフィスツアーや弊社主催の勉強会に参加してみてください！
          
</p>

</section>

---

### **ABC437参加者限定イベント**

<section>

<p>
LT会+懇親会をユニークビジョン 新宿オフィス（現地参加のみ）にて開催予定です！
</p>

<p>
「競技プログラミング」をテーマとして、登壇参加・聴講参加ともに募集いたします。

イベントへの参加を希望される方は、
<b>
必ず参加登録情報よりご回答ください
</b>
。コンテスト終了後、メールにて詳細をご案内いたします。

※希望者多数の場合には抽選とさせていただきます
  
</p>

#### **■ 開催概要**

<ul>

<li>
日時：
<strong>
2026年1月14日(水) 19:30~
</strong>

</li>

<li>
参加対象：本コンテスト参加者のみ
</li>

<li>
場所：ユニークビジョン 新宿オフィス（現地参加のみ）
</li>

</ul>

#### **■ ご登壇（LT会）について**

<ul>

<li>
時間： 5分 × 最大6名様
</li>

<li>
テーマ：競技プログラミングに関連すればなんでもOK
</li>

<li>
（例）今日から使える競プロTips、競プロ用実行環境構築の話、お気に入りのアルゴリズムなど
</li>

</ul>

<p>
当日は軽食をご用意してお待ちしております。是非お気軽にご参加ください！
</p>

</section>

---

### **配点**

<section>

<div>

<div>

<table>

<thead>

<tr>

<th>
問題
</th>

<th>
点数
</th>

</tr>

</thead>

<tbody>

<tr>

<td>
A
</td>

<td>
100
</td>

</tr>

<tr>

<td>
B
</td>

<td>
200
</td>

</tr>

<tr>

<td>
C
</td>

<td>
350
</td>

</tr>

<tr>

<td>
D
</td>

<td>
400
</td>

</tr>

<tr>

<td>
E
</td>

<td>
450
</td>

</tr>

<tr>

<td>
F
</td>

<td>
500
</td>

</tr>

<tr>

<td>
G
</td>

<td>
625
</td>

</tr>

</tbody>

</table>

</div>

</div>

</section>

---

### **賞品**

<section>

<p>
条件を満たす方へ抽選で25名にAmazonギフトカード10,000円分を進呈します。

未成年の参加者は、賞品の受け取りについて保護者の同意を得てください。

賞品に関する注意事項は<a href="https://drive.google.com/file/d/1PtaPRJ3SYyhhpGgt7ckosm0KULJKm4tF/view">こちら</a>をご確認ください。
          
</p>

</section>

<p>

</p>

<div>

<div>

<img src="https://img.atcoder.jp/abc283/f87431c5cca83ecad57d6da9d3be5d7f.png">

</img>

</div>

<span>
特別提供！
</span>

</div>

### **Amazonギフトカードが当たる！UV賞キャンペーン**

<section>

<p>
本コンテストでは上記賞品に加え、ユニークビジョン賞をお渡しします！

同社のサービスである<a href="https://www.uniquevision.co.jp/service/beluga-campaign/">Belugaキャンペーン for 𝕏</a>の「カスタムストーリー」機能を用いて、受賞者にはAmazonギフトカードを進呈します！
          
</p>

<p>
キャンペーン対象となる投稿は、2026年1月9日(金)11:00に<a href="https://twitter.com/uv_technology">@uv_technology</a>よりポストいたします。

是非、アカウントをフォローしてお待ちください！
          
</p>

</section>

#### **【賞品】**

<section>

<div>

<div>

<table>

<thead>

<tr>

<th>
金額
</th>

<th>
当選者数
</th>

</tr>

</thead>

<tbody>

<tr>

<td>
Amazonギフトカード 
<b>
10,000円
</b>
分
</td>

<td>
1名様
</td>

</tr>

<tr>

<td>
Amazonギフトカード 
<b>
2,000円
</b>
分
</td>

<td>
5名様
</td>

</tr>

<tr>

<td>
Amazonギフトカード
<b>
500円
</b>
分
</td>

<td>
60名様
</td>

</tr>

</tbody>

</table>

</div>

</div>

</section>

#### **【キャンペーン参加方法】**

<ol>

<li>
ユニークビジョン技術𝕏アカウント（<a href="https://twitter.com/uv_technology">@uv_technology</a>）をフォロー
  
</li>

<li>
キャンペーンポストから問題に挑戦！
</li>

<li>
成績をポストで応募完了
</li>

<li>
キャンペーン終了後一週間以内に、当選者のみにDMでご連絡（当選：66名）
</li>

</ol>

#### **【キャンペーン開催期間】**

<p>
2026年1月9日(金)11:00～1月15日(木)23:59
</p>

#### **【ユニークビジョン賞キャンペーンにおける注意事項】**
ユニークビジョン賞キャンペーンにおける注意事項は<a href="https://drive.google.com/file/d/1eT-sqEiCWJ2TgGy28jpaAe4I5mMz4qM0/view">こちら</a>をご確認ください。


        
---

### **ルール**

<section>

<ol>

<li>
コンテスト中に問題に正解すると点数を獲得できます。
</li>

<li>
順位は総合得点で決定します。
</li>

<li>
同点の場合は提出時間の早い人が上の順位になります。
</li>

<li>
誤答を提出するたびにペナルティが加算されます。このコンテストのペナルティは5分です。詳細は画面下部の「ルール」をご覧ください。
            
</li>

</ol>

<p>
このコンテストは full-feedback
            形式のコンテストです。コンテスト中に提出された結果だけで順位が決定します。
          
</p>

</section>

### **便利情報**

<ul>

<li>
<a href="https://atcoder.jp/">トップページ</a>
</li>

<li>
<a href="https://atcoder.jp/post/37">参加方法</a>
</li>

<li>
<a href="https://atcoder.jp/contests/practice">提出の練習ページ</a>
</li>

</ul>

</span>

</span>

</div>
