
<div>

<span>

<span>

<p>
配点 : $900$点
</p>

<div>

<section>

### **問題文**

<p>
$N$個の山が横一列に並んでいます．
左から $i$番目の山には $A_i$個の石があります．
</p>

<p>
FirstLeft くんと SecondRight くんがゲームをします．
FirstLeft くんから始めて，二人は交互に手番をプレイします．
それぞれの手番では，以下の操作を行います．
</p>

<ul>

<li>
FirstLeft くんの手番: FirstLeft くんは，石が $1$個以上ある山の中で最も
<strong>
左
</strong>
にある山から，$1$個以上の石を取り除く．
</li>

<li>
SecondRight くんの手番: SecondRight くんは，石が $1$個以上ある山の中で最も
<strong>
右
</strong>
にある山から，$1$個以上の石を取り除く．
</li>

</ul>

<p>
自分の手番で操作できなくなったプレイヤーの負けです．
二人が最適に行動する時，どちらが勝利するか判定してください．
</p>

<p>
$1$つの入力ファイルにつき，$T$個のテストケースを解いてください．
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq T \leq 100$
</li>

<li>
$1 \leq N \leq 100$
</li>

<li>
$1 \leq A_i \leq 10^9$
</li>

</ul>

</section>

</div>

---

<div>

<div>

<section>

### **入力**

<p>
入力は以下の形式で標準入力から与えられる．
入力の $1$行目は以下のとおりである．
</p>

<div>

$T$
</div>

<p>
そして，$T$個のテストケースが続く．
これらはそれぞれ以下の形式で与えられる．
</p>

<div>

$N$$A_1$$A_2$$\cdots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
各テストケースについて，FirstLeft くんが勝つ場合は `First`，SecondRight くんが勝つ場合は `Second`と出力せよ．
各テストケースごとに改行せよ．
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3
1
10
2
3 2
3
2 1 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

First
First
Second

</div>

<p>
例えば，$3$個目のゲームにおいて，次のようなシナリオが考えられます．
</p>

<ul>

<li>
FirstLeft くんが一番左の山から石を $2$個とる．山にある石の個数は $(0,1,2)$になる．
</li>

<li>
SecondRight くんが一番右の山から石を $1$個とる．山にある石の個数は $(0,1,1)$になる．
</li>

<li>
FirstLeft くんが真ん中の山から石を $1$個とる．山にある石の個数は $(0,0,1)$になる．
</li>

<li>
SecondRight くんが一番右の山から石を $1$個とる．山にある石の個数は $(0,0,0)$になる．
</li>

<li>
FirstLeft くんは操作を行うことができず，敗北する．
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
