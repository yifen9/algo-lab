
<div>

<span>

<span>

<p>
配点 : $700$点
</p>

<div>

<section>

### **問題文**

<p>
正整数 $N$および整数列 $A=(A_1,A_2,\ldots,A_N)$が与えられます．$A_i$は $-1$以上 $N-1$以下であり，$1\leq i\lt j\leq N$に対し，$A_i\neq -1$かつ $A_j\neq -1$ならば $A_i\neq A_j$です． 
</p>

<p>
次のクエリを $Q$回解いてください．
</p>

<ul>

<li>
整数 $l,r\ (1\leq l\leq r\leq N)$が与えられる．

$(0,1,\ldots,N-1)$の順列 $P=(P_1,P_2,\ldots,P_N)$であって，$A_i\neq -1\implies P_i=A_i$を満たすようなもの全てに対する $\mathrm{mex}(\lbrace P_l,P_{l+1}, \ldots,P_r\rbrace)$の総和を $998244353$で割った余りを求めよ．
</li>

</ul>

<details>

<summary>
$\mathrm{mex}(S)$とは
</summary>
非負整数からなる集合 $S$に対して，$S$に含まれない最小の非負整数を $\mathrm{mex}(S)$と定義します．

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N\leq 5000$
</li>

<li>
$1\leq Q\leq 5\times 10^5$
</li>

<li>
$-1\leq A_i\leq N-1$
</li>

<li>
$1\leq i\lt j\leq N$に対し，$A_i\neq -1$かつ $A_j\neq -1$ならば $A_i\neq A_j$
</li>

<li>
各クエリにおいて，$1\leq l\leq r\leq N$
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
入力は以下の形式で標準入力から与えられる．
</p>

<div>

$N$$Q$$A_1$$A_2$$\ldots$$A_N$$\mathrm{query}_1$$\mathrm{query}_2$$\vdots$$\mathrm{query}_Q$
</div>

<p>
各クエリは以下の形式で与えられる．
</p>

<div>

$l$$r$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$Q$行出力せよ．$i$行目には $\mathrm{query}_i$に対する答えを出力せよ．
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3 4
0 -1 -1
1 1
2 2
1 2
1 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2
0
3
6

</div>

<p>
$A_i\neq -1\implies P_i=A_i$であるような順列 $P$は $(0, 1, 2)$と $(0, 2, 1)$の $2$つです．したがって，各クエリの答えは以下のように求まります．
</p>

<ul>

<li>
$1$つ目のクエリの答えは $\mathrm{mex}(\lbrace 0\rbrace)+\mathrm{mex}(\lbrace 0\rbrace)=1+1=2$です．
</li>

<li>
$2$つ目のクエリの答えは $\mathrm{mex}(\lbrace 1\rbrace)+\mathrm{mex}(\lbrace 2\rbrace)=0+0=0$です．
</li>

<li>
$3$つ目のクエリの答えは $\mathrm{mex}(\lbrace 0,1\rbrace)+\mathrm{mex}(\lbrace 0,2\rbrace)=2+1=3$です．
</li>

<li>
$4$つ目のクエリの答えは $\mathrm{mex}(\lbrace 0,1,2\rbrace)+\mathrm{mex}(\lbrace 0,2,1\rbrace)=3+3=6$です．
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5 3
-1 2 -1 -1 1
1 4
3 5
1 5

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

6
8
30

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

15 1
-1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1
1 15

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

612227903

</div>

</section>

</div>

</span>

</span>

</div>
