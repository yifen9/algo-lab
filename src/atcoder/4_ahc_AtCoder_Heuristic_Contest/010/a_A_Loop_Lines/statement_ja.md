
<div>

<span>

<span>

<div>

<section>

### **ストーリー**

<p>
環状線が大好きな高橋くんは鉄道玩具で遊んでいる。
この玩具は、下図のように並べられた正方形の線路タイルを回転させることで線路を繋ぎ、その上を電車の模型を走らせるというものである。
高橋くんは電車の模型を2台持っているので、出来るだけ大きな環状線を2つ作ってほしい。
</p>

<table>

<tbody>

<tr>

<td>

<svg>

<rect>

</rect>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<defs>

<g>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

<g>

<path>

</path>

<path>

</path>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

</defs>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

</svg>

</td>

<td>

<svg>

<rect>

</rect>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<defs>

<g>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

<g>

<path>

</path>

<path>

</path>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

</defs>

<use>

</use>

<use>

</use>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<use>

</use>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<use>

</use>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<use>

</use>

<use>

</use>

</svg>

</td>

</tr>

<tr>

<td>
初期状態

</td>

<td>
右上と右中央を回転

</td>

</tr>

</tbody>

</table>

</section>

</div>

<div>

<section>

### **問題文**

<p>
$30\times 30$マスに並んだ線路タイルが与えられる。
タイルは回転したものを区別すると8種類あり、以下のように番号付ける。
</p>

<p>

<svg>

<rect>

</rect>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<text>
0

</text>

<text>
1

</text>

<text>
2

</text>

<text>
3

</text>

<text>
4

</text>

<text>
5

</text>

<text>
6

</text>

<text>
7

</text>

<defs>

<g>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

<g>

<path>

</path>

<path>

</path>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

</defs>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

</svg>

</p>

<p>
0から3番のタイルにはカーブした1本の線路、4番と5番のタイルにはカーブした2本の線路、6番と7番のタイルには直線の1本の線路が乗っている。
各タイルは90度ずつ回転させることが出来、反時計回りに90度回転させると次のようになる。
</p>

<p>

<svg>

<rect>

</rect>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<text>
1

</text>

<text>
2

</text>

<text>
3

</text>

<text>
0

</text>

<text>
5

</text>

<text>
4

</text>

<text>
7

</text>

<text>
6

</text>

<defs>

<g>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

<g>

<path>

</path>

<path>

</path>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

</defs>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

<use>

</use>

</svg>

</p>

<p>
線路に枝分かれはないため、各線路はパスもしくは閉路をなす。
閉路をなす線路の集合を「環状線」と呼び、その長さを、線路に沿って一周する際にタイルから隣接タイルへ移動する回数と定義する。
例えば、以下の環状線は7タイルからなるが、真ん中のタイルを二回通るため、長さは8である。
</p>

<p>

<svg>

<rect>

</rect>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<defs>

<g>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

<g>

<path>

</path>

<path>

</path>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

<line>

</line>

</g>

</defs>

<use>

</use>

<use>

</use>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<use>

</use>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<use>

</use>

<g>

<use>

</use>

</g>

<g>

<use>

</use>

</g>

<use>

</use>

<use>

</use>

</svg>

</p>

<p>
各タイルを回転させる回数を決定せよ。
</p>

</section>

</div>

<div>

<section>

### **得点**

<p>
出力に従ってタイルを回転させることで得られた環状線のうち、一番長いものの長さを$L_1$、二番目に長いものの長さを$L_2$とする(最長のものが複数ある場合は$L_1=L_2$)。
このとき、$L_1\times L_2$の得点が得られる。
環状線の個数が $1$以下の場合、そのテストケースの得点は $0$点となる。
</p>

<p>
テストケースは全部で 100 個あり、各テストケースの得点の合計が提出の得点となる。
1つ以上のテストケースで 
<span>
AC
</span>
以外の判定がされた場合、提出の得点は0点となる。
コンテスト時間中に得た最高得点で最終順位が決定され、コンテスト終了後のシステムテストは行われない。
同じ得点を複数の参加者が得た場合、その得点を獲得した提出の早い方が上位となる。
</p>

<p>
環状線の長さの求め方のヒント

</p>

<details>

<font color="red">疑似コードを更新しました。
</font>
環状線の長さは例えば以下のようにして計算できる。
タイルの状態が入った二次元配列を `tiles`とする。
方向を左上右下の順に0,1,2,3と番号付けると、座標の変化は配列 `di = [0, -1, 0, 1]`と `dj = [-1, 0, 1, 0]`で表される。
状態 `t`番のタイルに `d`の方向から侵入した際に次に向かうタイルの方向を `to[t][d]`、ただしそのような方向から侵入不可能な場合は`-1`とすると、以下のような二次元配列となる。
<p>

</p>

<div>

to = [
    [1, 0, -1, -1],
    [3, -1, -1, 0],
    [-1, -1, 3, 2],
    [-1, 2, 1, -1],
    [1, 0, 3, 2],
    [3, 2, 1, 0],
    [2, -1, 0, -1],
    [-1, 3, -1, 1],
];

</div>

<p>
位置 `(i, j)`のタイルに `d`の方向のタイルから侵入したとき、これらの組を以下のように更新出来る。
</p>

<div>

d2 = to[tiles[i][j]][d]; // 次のタイルの方向
if (d2 == -1) return 0; // 線路が途切れている
i += di[d2];
j += dj[d2];
if (i < 0 || i >= 30 || j < 0 || j >= 30) return 0; // 線路が途切れている
d = (d2 + 2) % 4; // 今居たタイルの方向

</div>

<p>
あとはこの処理を最初の位置と向き(同じタイルを二度通る可能性があることに注意)に戻ってくるまで繰り返せば、繰り返し回数が環状線の長さとなる。
</p>

<div>

// (si, sj) のタイルに sd 方向のタイルから侵入した状態からスタートして環状線の長さを求める
i = si;
j = sj;
d = sd;
loop {
    d2 = to[tiles[i][j]][d];
    if (d2 == -1) return 0;
    i += di[d2];
    j += dj[d2];
    if (i < 0 || i >= 30 || j < 0 || j >= 30) return 0;
    d = (d2 + 2) % 4;
    length += 1;
    if (i == si && j == sj && d == sd) return length;
}

</div>

</details>

</section>

</div>

---

<div>

<div>

<section>

### **入力**

<p>
入力は以下の形式で標準入力から与えられる。
</p>

<div>

$t_{0,0}$$\cdots$$t_{0,29}$$\vdots$$t_{29,0}$$\cdots$$t_{29,29}$
</div>

<p>
各 $t_{i,0}\cdots t_{i,29}$は長さ $30$の文字列である。
上から $i$$(0\leq i\leq 29)$番目、左から $j$$(0\leq j\leq 29)$番目のタイルを $(i, j)$と表す。
$t_{i,j}$はタイル $(i,j)$の状態を表す $0$以上 $7$以下の数字である。
</p>

</section>

</div>

<div>

<section>

### **出力**

<p>
タイル $(i,j)$を反時計回りに90度回転させる回数を $r_{i,j}$($0\leq r_{i,j}\leq 3$) としたとき、$30i+j$文字目が $r_{i,j}$となるような長さ $900$の文字列を1行に出力せよ。
</p>

<p>
解を複数回出力しても良い。複数出力された場合は一番最後のもののみが採点に用いられる。ビジュアライザでは複数出力された解の比較が可能である。
</p>

<p>
<a href="https://img.atcoder.jp/ahc010/d3a6c91ee76cb8.html?lang=ja&show=example">例を見る</a>
</p>

</section>

</div>

<div>

<section>

### **入力生成方法**

<p>
$L$以上 $U$以下の整数値を一様ランダムに生成する関数を $\mathrm{rand}(L,U)$で表す。
</p>

<p>
各 $t_{i,j}$はそれぞれ独立に以下のように生成される。
</p>

<ul>

<li>
25% の確率で $t_{i,j}=\mathrm{rand}(0, 3)$と生成する。
</li>

<li>
50% の確率で $t_{i,j}=\mathrm{rand}(4, 5)$と生成する。
</li>

<li>
25% の確率で $t_{i,j}=\mathrm{rand}(6, 7)$と生成する。
</li>

</ul>

</section>

</div>

<div>

<section>

### **ツール(入力ジェネレータ・ビジュアライザ)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc010/d3a6c91ee76cb8.html?lang=ja">Web版</a>: ローカル版より高性能でアニメーション表示が可能です。
</li>

<li>
<a href="https://img.atcoder.jp/ahc010/d3a6c91ee76cb8.zip">ローカル版</a>: 使用するには<a href="https://www.rust-lang.org/ja">Rust言語</a>のコンパイル環境をご用意下さい。
<ul>

<li>
<a href="https://img.atcoder.jp/ahc010/d3a6c91ee76cb8_windows.zip">Windows用のコンパイル済みバイナリ</a>: Rust言語の環境構築が面倒な方は代わりにこちらをご利用下さい。
</li>

</ul>

</li>

</ul>

<p>

<font color="red">
<strong>
コンテスト終了までビジュアライズ結果の共有は禁止されています。ご注意下さい。
</strong>
</font>

</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

436204751575440756541724746755
347475575404531645424640344414
556644445442451553264555436757
761235545455474254546631467555
356447405421445153457656535564
014274425356522445253477726464
311765446655556346633757446600
471744514426443445162555525455
616053450444473274742055767455
254124557527462423444450075637
046546764557475436717475255501
752005462554554414031525515356
452524742177476245065554577605
664465643742341605007655253777
444571276444165545442447340356
435050335454565235025507452540
467560030465475447567644441426
735730577745561712541450443547
472675153755474445700540444544
507472724556677621365747544757
535177720776402476665547676174
636275455643650141456764547131
164624553536572554544165746536
521574724335644274433544442556
576732703453654464555315065544
656244747015464523316444145414
555646775254464367454454067475
665624154657072514445150474444
570004746554540445465051654541
635504417414262014475547424275

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000

</div>

</section>

</div>

</span>

</span>

</div>
