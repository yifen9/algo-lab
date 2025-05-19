
<div>

<span>

<span>

<div>

<section>

### **問題文**

<p>
高橋君には、好きな文字列が $N$個ある。$i$番目の文字列は $S_i$であり、その好ましさは $P_i$である。各 $S_i$は、`a`〜`f`の6種類の英小文字のみから構成されている。
</p>

<p>
最近、高橋君は確率的に文字列を生成するモデルに興味を持っており、自分が好きな文字列が高い確率で現れるような生成モデル、
<strong>
Lovely Language Model (LLM)
</strong>
を設計したいと考えている。
</p>

<p>
この生成モデルは $M$個の状態から構成される。各状態 $i$（$0 \leq i < M$）には `a`〜`f`の 1 文字の英小文字 $C_i$を割り当てる。また、状態 $i$から状態 $j$への遷移確率を、パーセント単位の整数 $A_{i,j}$として設定する。これらはすべての $i$に対して次の条件を満たさなければならない：
</p>

<p>
\[
\sum_{j=0}^{M-1} A_{i,j} = 100
\]
</p>

<p>
このモデルは状態 $0$から開始し、長さ $L$の文字列を生成すると停止する。生成される文字列の 1 文字目には、初期状態 $0$に割り当てられた文字 $C_0$が使われる。その後は遷移確率に従って状態遷移を行い、各遷移先の状態に割り当てられた文字を順に出力していく。
</p>

<p>
このようにして生成された文字列において、各文字列 $S_i$が連続部分文字列として 
<strong>
1 回以上
</strong>
現れた場合、その好ましさ $P_i$を獲得する。好ましさの総和の期待値ができるだけ大きくなるように、文字割り当て $C_0, C_1, \dots, C_{M-1}$および遷移確率行列 $A$を設計せよ。
</p>

</section>

</div>

<div>

<section>

### **得点**

<p>
設計したモデルで長さ $L$の文字列を生成する場合に、各文字列 $S_i$が連続部分文字列として 
<strong>
1回以上
</strong>
含まれる確率を $Q_i$とする。
このとき、以下のスコアが得られる。
</p>

<p>
\[
\mathrm{round}\left(\sum_{i=0}^{N-1} P_i \cdot Q_i\right)
\]
</p>

<p>
合計で 150 個のテストケースがあり、各テストケースの得点の合計が提出の得点となる。
一つ以上のテストケースで不正な出力や制限時間超過をした場合、提出全体の判定が
<span>
WA
</span>
や
<span>
TLE
</span>
となる。
コンテスト時間中に得た最高得点で最終順位が決定され、コンテスト終了後のシステムテストは行われない。 同じ得点を複数の参加者が得た場合、提出時刻に関わらず同じ順位となる。
</p>

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

$N$$M$$L$$S_0$$P_0$$S_1$$P_1$$\vdots$$S_{N-1}$$P_{N-1}$
</div>

<ul>

<li>
$N$は文字列の数を表し、すべてのテストケースで $N = 36$に固定されている。
</li>

<li>
$M$はモデルの状態数であり、$M = 12$に固定されている。
</li>

<li>
$L$は生成する文字列の長さであり、$L = 10^6$に固定されている。
</li>

<li>
$S_i$は `a`〜`f`の英小文字からなる長さ $6 \leq |S_i| \leq 12$の文字列である。
</li>

<li>
好ましさ $P_i$は正の整数であり、$1 \leq P_i \leq 17000$を満たす。
</li>

<li>
すべての $S_i$は互いに異なる。
</li>

</ul>

</section>

</div>

<div>

<section>

### **出力**

<p>
設計したモデルにおいて、$i$番目の状態に割り当てる文字を $C_i$、状態 $i$から状態 $j$への遷移確率を $A_{i,j}$としたとき、以下の形式で標準出力に出力せよ。
</p>

<div>

$C_0$$A_{0,0}$$\cdots$$A_{0,M-1}$$\vdots$$C_{M-1}$$A_{M-1,0}$$\cdots$$A_{M-1,M-1}$
</div>

<ul>

<li>
各 $C_i$は `a`〜`f`のいずれかである。
</li>

<li>
各 $A_{i,j}$は $0 \leq A_{i,j} \leq 100$を満たす整数で、すべての $i$に対して \(\sum_{j=0}^{M-1} A_{i,j} = 100\) を満たさなければならない。
</li>

</ul>

<p>
解は複数回出力しても良い。
複数出力された場合、一番最後に出力された解のみが採点に用いられる。
Web版のビジュアライザを用いると、複数の解の比較が可能である。
</p>

<p>
<a href="https://img.atcoder.jp/ahc047/cHmFekjC.html?lang=ja&seed=0&output=sample">例を見る</a>
</p>

</section>

</div>

<div>

<section>

### **入力生成方法**

<p>
$\mathrm{rand}(L, U)$: $L$以上 $U$以下の整数値を一様ランダムに生成する。
</p>

#### **文字列 $S_i$の生成**

<p>
各 $S_i$の長さ $\ell_i$を $\ell_i = \mathrm{rand}(6, 12)$により決定し、長さ $\ell_i$の文字列を以下の手順で生成する：
</p>

<ul>

<li>
アルファベット `a`〜`f`から $\ell_i$回ランダムに選んで連結する。
</li>

<li>
同じ文字が複数回現れてもよい。
</li>

</ul>

<p>
生成した文字列 $S_i$がすでに生成した文字列と一致した場合、長さ $\ell_i$の生成からやり直す。
</p>

#### **好ましさ $P_i$の生成**

<p>
各文字列 $S_i$に対して、以下により対応する好ましさ $P_i$を生成する：
</p>

<ul>

<li>
最大値 $U_i = \left\lfloor 1.5^{2 \cdot \ell_i} \right\rfloor$を計算する。
</li>

<li>
$P_i = \mathrm{rand}(1, U_i)$により一様ランダムに生成する。
</li>

</ul>

<p>
このようにして、$N = 36$個の $(S_i, P_i)$の組を独立に生成する。
</p>

</section>

</div>

<div>

<section>

### **ツール(入力ジェネレータ・ビジュアライザ)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc047/cHmFekjC.html?lang=ja">Web版</a>: ローカル版より高性能でアニメーション表示が可能です。
</li>

<li>
<a href="https://img.atcoder.jp/ahc047/cHmFekjC.zip">ローカル版</a>: 使用するには<a href="https://www.rust-lang.org/ja">Rust言語</a>のコンパイル環境をご用意下さい。
<ul>

<li>
<a href="https://img.atcoder.jp/ahc047/cHmFekjC_windows.zip">Windows用のコンパイル済みバイナリ</a>: Rust言語の環境構築が面倒な方は代わりにこちらをご利用下さい。
</li>

</ul>

</li>

</ul>

<p>
コンテスト期間中に、ビジュアライズ結果の共有や、解法・考察に関する言及は禁止されています。ご注意下さい。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

36 12 1000000
acafbafdb 166
baeebdacd 86
baaffdcf 76
cfddcba 251
acdecbbfddaf 12423
ebcebe 107
feddecdb 373
acadbc 40
dcfaabebefcd 15639
fcebaade 438
cbefcedaaf 2468
efcfafcbcaac 4414
dbddcfa 96
cabacbdb 219
cbdeadcbad 3110
bbdeacbbe 894
deafadebdad 7067
dceedaacfefa 6453
deffecdee 280
cfffaaeca 651
aeffcbcfec 1021
ccefdcddadfd 6189
ffcdcb 91
afddebceadc 2283
ffebaff 258
aeceafebd 1235
fbbfec 83
fcdeceffbaf 1787
ddfffeb 188
bebffddaa 238
eedbfbaed 500
cacbccdbd 1346
cafbfbedcff 393
eccbdecdfefa 4423
fdfaddae 522
befebddfe 507

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

e 66 0 0 0 0 12 0 0 0 0 9 13
e 36 12 0 0 0 0 0 0 0 11 0 41
d 0 20 0 56 0 0 0 0 5 0 19 0
a 0 8 12 79 1 0 0 0 0 0 0 0
f 0 0 0 0 0 0 41 0 0 10 37 12
c 0 0 0 31 0 0 0 53 15 0 1 0
b 0 0 0 0 23 0 65 1 0 0 0 11
f 34 0 8 0 0 0 0 0 0 14 0 44
e 21 0 0 0 10 57 0 0 0 12 0 0
f 0 41 18 0 0 22 0 0 0 0 19 0
a 6 0 0 46 0 0 16 0 0 0 32 0
b 12 0 0 21 24 43 0 0 0 0 0 0

</div>

</section>

</div>

</span>

</span>

</div>
