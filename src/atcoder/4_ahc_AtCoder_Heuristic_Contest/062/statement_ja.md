
<div>

<span>

<span>

<canvas>

</canvas>

<script>
document.addEventListener('DOMContentLoaded', () => {
            const piCanvas = document.getElementById('piCanvas');
            const piCtx = piCanvas.getContext('2d');

            // πの数字列（小数点を含む）
            const PI_DIGITS = '3.141592653589793238462643383279502884197';
            let digitIdx = 0;

            let columns = [];

            const resizeCanvas = () => {
              piCanvas.width = window.innerWidth;
              piCanvas.height = window.innerHeight;
            };
            resizeCanvas();
            window.addEventListener('resize', resizeCanvas);

            const FONT_SIZE = 14;
            const CHAR_H = 20;
            // 表示領域: 左右 300px と 10% の小さい方
            const edgeX = () => {
              const band = Math.min(300, piCanvas.width * 0.1);
              if (band < 15) return -1;
              return Math.random() < 0.5
                ? 5 + Math.random() * (band - 10)
                : piCanvas.width - band + 5 + Math.random() * (band - 10);
            };

            // カラム生成（共有digitIdxから一気に取得）
            const spawnColumn = () => {
              const x = edgeX();
              if (x < 0) return;
              if (digitIdx >= PI_DIGITS.length) digitIdx = 0;
              const remaining = PI_DIGITS.length - digitIdx;
              const max = Math.min(4 + Math.floor(Math.random() * 10), remaining);
              const digits = PI_DIGITS.slice(digitIdx, digitIdx + max);
              digitIdx += max;
              columns.push({
                x,
                y: 30 + Math.random() * (piCanvas.height * 0.6),
                chars: [],
                digits,
                max,
                timer: 0,
                interval: 5 + Math.floor(Math.random() * 8),
                hue: 335 + Math.random() * 20
              });
            };

            // カラム更新＆描画
            const updateColumns = () => {
              piCtx.clearRect(0, 0, piCanvas.width, piCanvas.height);
              piCtx.font = `${FONT_SIZE}px "Courier New", monospace`;
              piCtx.textAlign = 'center';

              for (let i = columns.length - 1; i >= 0; i--) {
                const col = columns[i];

                col.timer++;
                if (col.timer >= col.interval && col.chars.length < col.max) {
                  col.timer = 0;
                  col.chars.push({ ch: col.digits[col.chars.length], age: 0, opacity: 1 });
                }

                let alive = false;
                const complete = col.chars.length >= col.max;

                for (let j = 0; j < col.chars.length; j++) {
                  const c = col.chars[j];
                  c.age++;
                  const isHead = j === col.chars.length - 1 && !complete;

                  if (complete) {
                    const delay = j * 6;
                    if (c.age > 40 + delay) c.opacity = Math.max(0, c.opacity - 0.015);
                  }

                  if (c.opacity <= 0) continue;
                  alive = true;

                  const cy = col.y + j * CHAR_H;
                  const bright = isHead ? 85 : Math.max(35, 70 - c.age * 0.4);

                  if (isHead) {
                    piCtx.shadowColor = `hsla(${col.hue}, 90%, 70%, ${c.opacity * 0.6})`;
                    piCtx.shadowBlur = 10;
                  } else {
                    piCtx.shadowBlur = 0;
                  }

                  piCtx.fillStyle = `hsla(${col.hue}, 75%, ${bright}%, ${c.opacity})`;
                  piCtx.fillText(c.ch, col.x, cy);
                }

                piCtx.shadowBlur = 0;
                if (!alive && complete) columns.splice(i, 1);
              }
            };

            let frame = 0;
            const animate = () => {
              frame++;
              if (frame % 40 === 0 && columns.length < 15) spawnColumn();
              updateColumns();
              requestAnimationFrame(animate);
            };
            animate();
          });

        
</script>

### **コンテスト情報**

<section>

<ul>

<li>
writer: <a href="https://atcoder.jp/contests/ahc062/users/Kiri8128">
<img src="https://atcoder.jp//img.atcoder.jp/assets/icon/crown_bronze.png">

</img>

<span>
Kiri8128
</span>
</a>
</li>

<li>
このコンテストは <a href="https://atcoder.jp/posts/1380">AHCレーティング(v2)</a>の対象です。
</li>

<li>
このコンテストは <a href="https://atcoder.jp/posts/1635">AWTF2027</a>選考の対象です。
</li>

</ul>

</section>

---

### **コンテスト概要**

<section>

<div>

<img src="https://drive.google.com/thumbnail?id=1MUwqugOFRGyKSiMeaB4IHqoDgJvQk6mE&sz=w1000">

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
<a href="https://atcoder.jp/contests/ahc062#office-event">AHC062参加者限定イベント
        
<svg>

<polyline>

</polyline>

</svg>
</a><a href="https://atcoder.jp/contests/ahc062#campaign">Amazonギフトカードが当たる！UV賞キャンペーン
        
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
このコンテスト開催を通じて、技術が好きなAtCoderユーザーの皆様にユニークビジョンのことを知っていただき、是非とも一緒に技術で世の中を変えていく仲間となっていただきたいと考えています。
  
</p>

<p>
私たちは企業とファンをつなぐSNSマーケティングツールを開発・提供しているテクノロジーカンパニーです。
  
</p>

<p>
SNSは情報の拡散が非常に速く、影響力も大きいメディアです。当社のクライアントである大手企業がSNSで実施するキャンペーンは、品質やスピードの面でシビアなものがほとんどです。
必ずしも唯一の正解があるわけではなく、トレードオフを考えながら改善を積み重ねていく――こうした課題は、ヒューリスティックコンテストで求められる考え方と非常に近いものだと感じています。
  
</p>

<p>
ユニークビジョンでは、競技プログラミングで培われた
<b>
「仮説を立て、試行錯誤しながらより良い解を目指す力」「実装と改善を高速に回す力」
</b>
を活かしながら、サービスの開発に取り組むことができます。
 
</p>

<p>
社内には向上心の高いエンジニアが多く、競プロから最新技術まで活発に議論されています。ヒューリスティックな問題解決を楽しめる皆様とともに
<b>
技術格差を、解く。潜在能力を、放つ
</b>
というミッションを体現するため、一緒にチャレンジできることを楽しみにしています。
     
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
、TypeScript
    
</li>

</ul>

#### **フレームワーク**

<ul>

<li>
axum, Vue.js
</li>

</ul>

#### **クラウドプラットフォーム**

<ul>

<li>
Amazon Web Services (AWS)
            
</li>

</ul>

#### **インフラ構成管理**

<ul>

<li>
AWS Cloud Development Kit (AWS CDK)
</li>

</ul>

#### **プロジェクト管理**

<ul>

<li>
GitHub
            
</li>

</ul>

#### **AIエージェント**

<ul>

<li>
Claude Code、GitHub Copilot
</li>

</ul>

</section>

---

### **社内競技プログラミング部員のメッセージ**

<section>

<p>
数年前まで社内に競技プログラマーはほとんどいませんでしたが、年々仲間が増え、今では15名以上が在籍しています。
有志で競技プログラミング部を作り、出場したいコンテストの仲間を募ったり、問題の振り返りをしたりという活動をしています！
          
</p>

<p>
競プロユーザーがいなかった時代もあったので、社員同士でチーム戦のコンテストに出たときはとても嬉しかったです。
実際の業務においても、「どう改善すればより良くなるか」を考え続ける姿勢は、ヒューリスティックな課題解決そのものだと感じています。
          
</p>

<p>
共通の話題があるので打ち解けるのも早く、AtCoderさんの本社が近いことも密かな自慢ポイントです(笑)

気になった方は是非、キャンペーン後のLT会やUV Study（勉強会）などで遊びに来てください！
          
</p>

</section>

<div>

<img src="https://img.atcoder.jp/abc334/Competitive_programming_club.png">

</img>

</div>

---

### **AHC062参加者限定イベント**

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
2026年4月8日(水) 19:30~
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
（例）今日から使える競プロTips、競プロ用実行環境構築の話、お気に入りの解法など
</li>

</ul>

<p>
当日は軽食をご用意してお待ちしております。是非お気軽にご参加ください！
</p>

</section>

---

### **賞品**

### **一般賞**

<section>

<div>

<div>

<table>

<thead>

<tr>

<th>
順位
</th>

<th>
賞品
</th>

</tr>

</thead>

<tbody>

<tr>

<td>
1位
</td>

<td>
20,000円
</td>

</tr>

<tr>

<td>
2位
</td>

<td>
15,000円
</td>

</tr>

<tr>

<td>
3位
</td>

<td>
10,000円
</td>

</tr>

<tr>

<td>
4位
</td>

<td>
5,000円
</td>

</tr>

<tr>

<td>
5～100位から抽選で25名
</td>

<td>
3,000円
</td>

</tr>

</tbody>

</table>

</div>

</div>

</section>

### **学生賞**

<section>

<div>

<div>

<table>

<thead>

<tr>

<th>
順位
</th>

<th>
賞品
</th>

</tr>

</thead>

<tbody>

<tr>

<td>
1位
</td>

<td>
20,000円
</td>

</tr>

<tr>

<td>
2位
</td>

<td>
15,000円
</td>

</tr>

<tr>

<td>
3位
</td>

<td>
10,000円
</td>

</tr>

<tr>

<td>
4位
</td>

<td>
5,000円
</td>

</tr>

<tr>

<td>
5～100位から抽選で25名
</td>

<td>
3,000円
</td>

</tr>

</tbody>

</table>

</div>

</div>

</section>

<section>

<p>

</p>

<ul>

<li>
条件を満たす方へAmazonギフトカードを進呈します。各金額については上記の表をご確認ください。
</li>

</ul>

<ul>

<li>
未成年の参加者は、賞品の受け取りについて保護者の同意を得てください。
</li>

</ul>

<ul>

<li>
5～100位の方は、条件を満たした方へ抽選で25名に3,000円を贈呈します。
</li>

</ul>

<ul>

<li>
賞品に関する注意事項は<a href="https://drive.google.com/file/d/12RFJb3NGoBgFN7uGAPY5dviiIIDqEj-_/view?usp=sharing">こちら</a>をご確認ください。
</li>

</ul>

<p>

</p>

</section>

<p>

</p>

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
キャンペーン対象となる投稿は、2026年3月27日(金)11:00に<a href="https://twitter.com/uv_technology">@uv_technology</a>よりポストいたします。

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
1,000円
</b>
分
</td>

<td>
40名様
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
キャンペーン終了後一週間以内に、当選者のみにDMでご連絡（当選：40名）
</li>

</ol>

#### **【キャンペーン開催期間】**

<p>
2026年3月27日(金)11:00～4月2日(木)23:59
</p>

#### **【ユニークビジョン賞キャンペーンにおける注意事項】**
ユニークビジョン賞キャンペーンにおける注意事項は<a href="https://drive.google.com/file/d/1eT-sqEiCWJ2TgGy28jpaAe4I5mMz4qM0/view">こちら</a>をご確認ください。


        
---

### **ルール**

<section>

<ul>

<li>
問題は1問です。AtCoderで使用できるすべてのプログラミング言語を使用可能です。
</li>

<li>
誤提出・再提出のペナルティはありませんが、解答を提出する際は前回の提出から
<strong>
5分以上の間隔
</strong>
を開ける必要があります。
                
</li>

<li>
コンテストは個人戦です。2人以上で結託し、解答する行為は禁止しております。
</li>

<li>

<strong>
コンテスト終了前に、問題の考察や解答を公開する行為は禁止しております。
</strong>
ただし、提供されたツール類の動かし方に関する情報は自由に共有して構いません。
</li>

</ul>

</section>

### **メニューについて**

<section>

<p>
なお、上メニューバーの各ボタンの機能は、以下の通りです。
            
</p>

<ul>

<li>
<a href="https://atcoder.jp/contests/ahc062#">トップ</a>: 現在閲覧中のページです。
</li>

<li>
<a href="https://atcoder.jp/contests/ahc062/assignments">問題</a>: コンテストの問題の閲覧ができます。
</li>

<li>
<a href="https://atcoder.jp/contests/ahc062/submit">提出</a>: コンテストの問題に対する、解答ソースコードを提出することが出来ます。
</li>

<li>
<a href="https://atcoder.jp/contests/ahc062/clarifications">質問</a>: コンテスト全体、および各問題に対して、コンテスト中に質問し、その回答を閲覧することが出来ます。
</li>

<li>
<a href="https://atcoder.jp/contests/ahc062/submissions/me">結果</a>: 今までに自分が提出した解答を閲覧することができます。また、コンテスト終了後には他の参加者の解答状況を閲覧することが出来ます。
                
</li>

<li>
<a href="https://atcoder.jp/contests/ahc062/standings">順位表</a>: 現在のコンテストの順位表が閲覧できます。
</li>

</ul>

</section>

### **その他**

<section>

<p>
<a href="https://atcoder.jp/contests/ahc062/tos">利用規約</a>、<a href="https://atcoder.jp/contests/ahc062/rules">ルール</a>、<a href="https://atcoder.jp/contests/ahc062/glossary">用語集</a>、<a href="https://atcoder.jp/contests/ahc062/faq">よくある質問</a>をご一読下さいませ。
            
</p>

</section>

</span>

</span>

</div>
