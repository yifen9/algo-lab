
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
整数 $N,M$が与えられるので、 $\lfloor N/M \rfloor$を $\color{red}{10007}$で割った余りを求めてください。

ここで、 $\lfloor x \rfloor$は $x$以下で最大の整数を表します。 例えば、 $\lfloor 3.14 \rfloor=3, \lfloor 10 \rfloor = 10$です。
</p>

<p>
但し、この問題では $N$は直接与えられず、ランレングス圧縮された形で与えられます。

具体的には、 $N$は $K$個の「数字 $c_i$と整数 $l_i$の組」からなる列で表現されます。

元の $N$を復元するには、以下の手順を用います。
</p>

<ul>

<li>
最初、文字列 $S$を空文字列とする。
</li>

<li>
$i=1,2,\dots,K$について、以下を繰り返す。
<ul>

<li>
$S$の末尾に数字 $c_i$を $l_i$個付け加える。
</li>

</ul>

</li>

<li>
最終的な $S$をひとつの整数として解釈したとき、その整数が $N$である。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \le M \le 10^4$
</li>

<li>
$1 \le K \le 10^5$
</li>

<li>
$c_i$は $0,1,2,3,4,5,6,7,8,9$いずれかの数字
</li>

<li>
$1 \le l_i \le 10^9$
</li>

<li>
$c_1 \neq 0$
</li>

<li>
$M,K,l_i$は整数
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

$K$$M$$c_1$$l_1$$c_2$$l_2$$\vdots$$c_K$$l_K$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

6 7
3 1
1 1
6 1
2 2
7 2
6 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3797

</div>

<p>
この入力では $N=316227766,M=7$です。

$\lfloor 316227766/7 \rfloor = 45175395$であり、これを $10007$で割った余りである $3797$が最終的な答えとなります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

1 1
1 1

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10 9999
9 419921892
9 923650333
6 476449815
1 8837775
2 141135534
5 462618481
3 202652735
0 771538044
4 321458589
0 570032864

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

8437

</div>

</section>

</div>

</span>

</span>

</div>
