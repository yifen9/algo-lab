
<div>

<span>

<span>

<div>

<section>

### **ストーリー**

<p>
AtCoder社の高橋社長は明日のハロウィンに向けて準備をしている。
AtCoder社のハロウィンは、仮装をした高橋社長が Trick or treat と唱えて、$100$人の従業員から順番に1つずつキャンディーを貰うイベントである。
高橋社長は格子状に $10\times 10$個のキャンディーが入る正方形の箱を用意し、各従業員はキャンディーが重ならないように空いているスペースにキャンディーを入れていく。
キャンディーはイチゴ味、スイカ味、パンプキン味の $3$種類があり、事前調査によって各従業員がどの味のキャンディーを入れるかは分かっているが、入れる場所は分からない。
几帳面な高橋社長は、キャンディーを一つ受け取る毎に、箱を前後左右に一度だけ傾けることでキャンディーを動かし、最終的に出来るだけ同じ種類のキャンディー同士が固まっているようにしたいと考えている。
傾け方を決めるプログラムを作成することで高橋社長の手伝いをして欲しい。
</p>

<figure>

<img src="https://img.atcoder.jp/ahc015/b639c75d_1.gif">

</img>

<figcaption>
$5\times 5$の場合の例
</figcaption>

</figure>

</section>

</div>

<div>

<section>

### **問題文**

<p>
格子状に $10\times 10$個のキャンディーが入る箱がある。
箱は初期状態では空であり、$100$個のキャンディーを順番に入れていく。
キャンディーは全部で $3$種類の味があり、事前に $t$番目に受け取るキャンディーの味の種類 $f_t (1\leq f_t\leq 3)$が分かっている。
一方で、どの位置に入るかは事前には分からず、空いているマスの中から一様ランダムに選ばれる。
キャンディーを受け取る順番は固定で、変更することは出来ない。
</p>

<p>
キャンディーを一つ受け取る度に、箱を前後左右にちょうど一回だけ傾ける。
箱を傾けると、各キャンディーがその方向に、端か他のキャンディーにぶつかるまで一斉に移動する。
例えば、左図の状態で箱を前方に傾けると、右図の状態となる。
</p>

<p>

<img src="https://img.atcoder.jp/ahc015/b639c75d_2.png">

</img>

<img src="https://img.atcoder.jp/ahc015/b639c75d_3.png">

</img>

</p>

</section>

</div>

<div>

<section>

### **得点**

<p>
以下のようにキャンディーの連結性を定義し、連結成分分解を考える。
</p>

<blockquote>

<p>
2つのキャンディーは、同じ味であり、かつ、前後左右に同じ味のキャンディーのみを通って互いに到達可能な場合に、またその場合に限り、連結である。
</p>

</blockquote>

<p>
例えば以下の図の状態は大きさ $\{1, 1, 2, 2, 4, 6, 9\}$の $7$個の連結成分からなる。
</p>

<p>

<img src="https://img.atcoder.jp/ahc015/b639c75d_4.png">

</img>

</p>

<p>
最終的に100個のキャンディーを受け取った状態における連結成分の大きさのリストを $n_1,\cdots,n_k$とし、$i$番の味のキャンディーの総数を $d_i$とした時、以下のスコアが得られる。
</p>

<p>
\[\mathrm{round}\left(10^6\times\frac{\sum_{i=1}^k n_i^2}{\sum_{i=1}^3 d_i^2}\right)\]
</p>

<p>
出来るだけ高得点が得られるように傾け方を決定するプログラムを作成せよ。
</p>

<p>
テストケースは全部で 200 個あり、各テストケースの得点の合計が提出の得点となる。
一つ以上のテストケースで不正な出力や制限時間超過をした場合、提出全体の判定が
<span>
WA
</span>
や
<span>
TLE
</span>
となる。
コンテスト時間中に得た最高得点で最終順位が決定され、コンテスト終了後のシステムテストは行われない。 同じ得点を複数の参加者が得た場合、提出時刻に関わらず同じ順位となる(従来の短期AHCから変更となっているので注意)。
</p>

</section>

</div>

<div>

<section>

### **入出力**

<p>
まずはじめに、各キャンディーの味の情報が以下の形式で標準入力から与えられる。
</p>

<div>

$f_1$$f_2$$\cdots$$f_{100}$
</div>

<p>
各 $f_t$は $t$番目に受け取るキャンディーの味を表す、$1$以上 $3$以下の整数値である。
</p>

<p>
上記の情報を読み込んだら、以下の処理を $100$回繰り返す。
</p>

<p>
$t$($1\leq t\leq 100$) 回目の処理ではまず、$1$以上 $101-t$以下の整数値 $p_t$が一つ標準入力から与えられる。
下図の例のように、前から後ろ、左から右の優先順位で空きマスに $1$から $101-t$の番号を順番に付けたとき、$p_t$番目の空きマスに $t$個目のキャンディーが入れられることを表している。
</p>

<p>

<img src="https://img.atcoder.jp/ahc015/b639c75d_5.png">

</img>

</p>

<p>
$p_t$の情報を読み込んだら、前後左右をそれぞれ `F`、`B`、`L`、`R`で表して、どの方向へ傾けるかを一文字で標準出力に出力せよ。

<font color="red">
<strong>
出力の後には改行をし、更に標準出力を flush しなければならない。
</strong>
</font>
そうしない場合、
<span>
TLE
</span>
となる可能性がある。

<font color="red">
<strong>
$t$回目の方向を出力するまで、$p_{t+1}$の入力は与えられないので注意せよ。
</strong>
</font>
$100$回目はどの方向に傾けても同じであるため、出力をしてもしなくても良い。
</p>

#### **例**

<table>

<thead>

<tr>

<th>
$t$
</th>

<th>
Input
</th>

<th>
Output
</th>

</tr>

</thead>

<tbody>

<tr>

<td>
事前情報
</td>

<td>

<div>

2 2 1 3 1 2 1 2 1 $\cdots$3
</div>

</td>

<td>

</td>

</tr>

<tr>

<td>
1
</td>

<td>

<div>

3
</div>

</td>

<td>

<div>

R
</div>

</td>

</tr>

<tr>

<td>
2
</td>

<td>

<div>

98
</div>

</td>

<td>

<div>

B
</div>

</td>

</tr>

<tr>

<td>
$\vdots$
</td>

<td>

</td>

<td>

</td>

</tr>

<tr>

<td>
100
</td>

<td>

<div>

1
</div>

</td>

<td>

<div>

L
</div>

</td>

</tr>

</tbody>

</table>

<p>
<a href="https://img.atcoder.jp/ahc015/b639c75d.html?lang=ja&seed=0&output=R%0D%0AB%0D%0AB%0D%0AR%0D%0AF%0D%0AR%0D%0AF%0D%0AR%0D%0AR%0D%0AF%0D%0AB%0D%0AL%0D%0AB%0D%0AL%0D%0AF%0D%0AF%0D%0AB%0D%0AF%0D%0AB%0D%0AL%0D%0AL%0D%0AL%0D%0AL%0D%0AB%0D%0AF%0D%0AF%0D%0AR%0D%0AR%0D%0AF%0D%0AL%0D%0AL%0D%0AB%0D%0AL%0D%0AL%0D%0AL%0D%0AB%0D%0AL%0D%0AR%0D%0AF%0D%0AL%0D%0AB%0D%0AL%0D%0AF%0D%0AF%0D%0AF%0D%0AL%0D%0AL%0D%0AR%0D%0AB%0D%0AB%0D%0AF%0D%0AL%0D%0AF%0D%0AR%0D%0AB%0D%0AL%0D%0AF%0D%0AF%0D%0AR%0D%0AL%0D%0AR%0D%0AL%0D%0AR%0D%0AR%0D%0AB%0D%0AR%0D%0AB%0D%0AR%0D%0AR%0D%0AF%0D%0AB%0D%0AF%0D%0AR%0D%0AR%0D%0AF%0D%0AB%0D%0AF%0D%0AB%0D%0AF%0D%0AR%0D%0AB%0D%0AF%0D%0AF%0D%0AF%0D%0AB%0D%0AB%0D%0AL%0D%0AL%0D%0AR%0D%0AF%0D%0AB%0D%0AL%0D%0AB%0D%0AF%0D%0AB%0D%0AR%0D%0AF%0D%0AF%0D%0AL%0D%0AL%0D%0A">例を見る</a>
</p>

</section>

</div>

<div>

<section>

### **入力生成方法**

<p>
$L$以上 $U$以下の整数値を一様ランダムに生成する関数を $\mathrm{rand}(L,U)$で表す。
各 $f_t$は $\mathrm{rand}(1,3)$により生成される。
各 $p_t$は $\mathrm{rand}(1,101-t)$により生成される。
</p>

</section>

</div>

<div>

<section>

### **ツール(入力ジェネレータ・ビジュアライザ)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc015/b639c75d.html?lang=ja">Web版</a>: ローカル版より高性能でアニメーション表示と手動プレイが可能です。
</li>

<li>
<a href="https://img.atcoder.jp/ahc015/b639c75d.zip">ローカル版</a>: 使用するには<a href="https://www.rust-lang.org/ja">Rust言語</a>のコンパイル環境をご用意下さい。
<ul>

<li>
<a href="https://img.atcoder.jp/ahc015/b639c75d_windows.zip">Windows用のコンパイル済みバイナリ</a>: Rust言語の環境構築が面倒な方は代わりにこちらをご利用下さい。
</li>

</ul>

</li>

</ul>

<p>
コンテスト期間中に、ビジュアライズ結果の共有や、解法・考察に関する言及は禁止されています。ご注意下さい。
</p>

</section>

</div>

</span>

</span>

</div>
