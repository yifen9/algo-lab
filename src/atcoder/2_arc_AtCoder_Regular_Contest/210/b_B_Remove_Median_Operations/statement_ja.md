
<div>

<span>

<span>

<p>
配点 : $600$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の整数列 $A=(A_1,A_2,\ldots,A_N)$および，長さ $M$の整数列 $B=(B_1,B_2,\ldots,B_M)$が与えられます．ここで $N$は
<strong>
偶数
</strong>
です．
</p>

<p>
$Q$個のクエリが与えられます．$q$個目のクエリの情報は整数の $3$つ組 $(t_q,i_q,x_q)$として与えられ，その内容は以下の通りです．
</p>

<ul>

<li>
$t_q=1$の場合：このとき $1\leq i_q\leq N$である．このクエリでは $A_{i_q}$を $x_q$に変更する．
</li>

<li>
$t_q=2$の場合：このとき $1\leq i_q\leq M$である．このクエリでは $B_{i_q}$を $x_q$に変更する．
</li>

</ul>

<p>
クエリを処理するたびに，次の小問題の答を求めてください．
</p>

<blockquote>

<p>
多重集合 $X$を $X=\lbrace A_1,A_2,\ldots,A_N\rbrace$で初期化します．
$j=1,2,\ldots,M$に対して次の操作を行います：
</p>

<ul>

<li>
$X$に $B_j$を挿入する．その後，$X$の中央値を $X$からひとつ削除する．
</li>

</ul>

<p>
すべての操作が終了したときの $X$の要素の総和を求めてください．
</p>

</blockquote>

<details>

<summary>
中央値とは
</summary>

<p>
$N$が偶数であるとき，$N+1$個の要素を持つ多重集合 $X$の中央値とは，$X$の要素のうち昇順で $\left(1+\frac{N}{2}\right)$番目の値です．

</p>

<p>
例えば $X=\lbrace 1, 3, 4, 5, 8\rbrace$の中央値は $4$，$X=\lbrace 2,2,2\rbrace$の中央値は $2$です．

</p>

<p>
本問題において，中央値を考える多重集合は常に要素数が奇数であることに注意してください．

</p>

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N,M,Q\leq 2\times 10^5$
</li>

<li>
$N$は偶数．
</li>

<li>
$1\leq A_i\leq 10^9$
</li>

<li>
$1\leq B_i\leq 10^9$
</li>

<li>
$t_q\in\lbrace 1,2\rbrace$
</li>

<li>
$t_q=1$ならば $1\leq i_q\leq N$
</li>

<li>
$t_q=2$ならば $1\leq i_q\leq M$
</li>

<li>
$1\leq x_q\leq 10^9$
</li>

<li>
入力される値はすべて整数．
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
入力は以下の形式で標準入力から与えられます．
</p>

<div>

$N$$M$$Q$$A_1$$A_2$$\cdots$$A_N$$B_1$$B_2$$\cdots$$B_M$$t_1$$i_1$$x_1$$\vdots$$t_Q$$i_Q$$x_Q$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$Q$行出力してください．$q$行目には，$q$個目のクエリを処理した直後における小問題の答を出力してください．
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 2 2
5 1 4 3
1 2
1 3 3
2 1 5

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

10
13

</div>

<p>
まず $1$個目のクエリによって，$A=(5,1,3,3)$, $B=(1,2)$となります．この場合，小問題の操作は次のように進行します．
</p>

<ul>

<li>
$X=\lbrace 5,1,3,3\rbrace=\lbrace 1,3,3,5\rbrace$で初期化される．
</li>

<li>
$X$に $B_1=1$を挿入し，$X=\lbrace 1,1,3,3,5\rbrace$となる．その後，$X$の中央値をひとつ削除して $X=\lbrace 1,1,3,5\rbrace$となる．
</li>

<li>
$X$に $B_2=2$を挿入し，$X=\lbrace 1,1,2,3,5\rbrace$となる．その後，$X$の中央値をひとつ削除して $X=\lbrace 1,1,3,5\rbrace$となる．
</li>

</ul>

<p>
すべての操作が終了した時点での $X$の要素の総和は $1+1+3+5=10$です．
</p>

<p>
次に $2$個目のクエリによって，$A=(5,1,3,3)$, $B=(5,2)$となります．この場合，小問題の操作は次のように進行します．
</p>

<ul>

<li>
$X=\lbrace 5,1,3,3\rbrace=\lbrace 1,3,3,5\rbrace$で初期化される．
</li>

<li>
$X$に $B_1=5$を挿入し，$X=\lbrace 1,3,3,5,5\rbrace$となる．その後，$X$の中央値をひとつ削除して $X=\lbrace 1,3,5,5\rbrace$となる．
</li>

<li>
$X$に $B_2=2$を挿入し，$X=\lbrace 1,2,3,5,5\rbrace$となる．その後，$X$の中央値をひとつ削除して $X=\lbrace 1,2,5,5\rbrace$となる．
</li>

</ul>

<p>
すべての操作が終了した時点での $X$の要素の総和は $1+2+5+5=13$です．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

6 7 5
7 1 2 5 5 3
4 2 5 1 3 3 8
2 1 3
2 7 1
1 3 6
2 4 2
1 5 1

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

24
20
21
22
21

</div>

</section>

</div>

</span>

</span>

</div>
