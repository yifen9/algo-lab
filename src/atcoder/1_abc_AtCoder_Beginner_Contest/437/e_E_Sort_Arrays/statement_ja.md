
<div>

<span>

<span>

<p>
配点 : $450$点
</p>

<div>

<section>

### **問題文**

<p>
$N+1$個の数列 $A_0, A_1, \ldots, A_{N}$があります。$A_i$は以下のように定義されます。
</p>

<ul>

<li>
$A_0$は空の数列
</li>

<li>
$A_i\ (1\leq i\leq N)$は数列 $A_{x_i}\ (0\leq x_i\lt i)$の末尾に整数 $y_i$を追加することで得られる数列
</li>

</ul>

<p>
以下の条件を満たす $(1,2,\ldots,N)$の順列 $P=(P_1, P_2,\ldots,P_N)$を求めてください。
</p>

<ul>

<li>
$i = 1,2,\ldots,N-1$に対して、以下のいずれかが成り立つ。
<ul>

<li>
$A_{P_i}$は辞書順で $A_{P_{i+1}}$より小さい。
</li>

<li>
$A_{P_i}= A_{P_{i+1}}$かつ $P_i\lt P_{i+1}$
</li>

</ul>

</li>

</ul>

<p>
言い換えると、$A_1,A_2,\ldots,A_N$を辞書順で小さいものから順に並べたとき（等しい列が複数ある場合には添え字が小さいものを先にするように並べる）、その並びに現れる添え字の列が $P$です。
</p>

<details>

<summary>
数列の辞書順とは？
</summary>

<p>
数列 $S = (S_1,S_2,\ldots,S_{|S|})$が数列 $T = (T_1,T_2,\ldots,T_{|T|})$より
<strong>
辞書順で小さい
</strong>
とは、下記の 1. と 2. のどちらかが成り立つことを言います。
ここで、$|S|, |T|$はそれぞれ $S, T$の長さを表します。
</p>

<ol>

<li>
$|S| \lt |T|$かつ $(S_1,S_2,\ldots,S_{|S|}) = (T_1,T_2,\ldots,T_{|S|})$。 
</li>

<li>
ある整数 $1 \leq i \leq \min\lbrace |S|, |T| \rbrace$が存在して、下記の $2$つがともに成り立つ。

<ul>

<li>
$(S_1,S_2,\ldots,S_{i-1}) = (T_1,T_2,\ldots,T_{i-1})$
</li>

<li>
$S_i$が $T_i$より（数として）小さい。
</li>

</ul>

</li>

</ol>

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N\leq 3\times 10^5$
</li>

<li>
$0\leq x_i\lt i$
</li>

<li>
$1\leq y_i\leq 10^9$
</li>

<li>
入力は全て整数
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
入力は以下の形式で標準入力から与えられる。
</p>

<div>

$N$$x_1$$y_1$$x_2$$y_2$$\vdots$$x_N$$y_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$P_1, P_2, \ldots, P_N$を空白区切りで一行で出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4
0 2
0 1
2 2
0 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2 4 3 1

</div>

<p>
$A_1 = (2), A_2 = (1), A_3 = (1, 2), A_4 = (1)$なので $P=(2,4,3,1)$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5
0 1
0 1
0 1
0 1
0 1

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1 2 3 4 5

</div>

<p>
$A_1 = A_2 = A_3 = A_4 = A_5 = (1)$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10
0 305186313
1 915059758
0 105282054
1 696409999
3 185928366
3 573289179
6 254538849
3 105282054
5 696409999
8 168629803

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

3 8 10 5 9 6 7 1 4 2

</div>

</section>

</div>

</span>

</span>

</div>
