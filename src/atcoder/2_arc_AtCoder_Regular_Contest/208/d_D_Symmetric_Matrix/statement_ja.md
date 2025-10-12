
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
各要素が $1$以上 $N$以下であるような長さ $N$の整数列 $Y=(Y_1,Y_2,\ldots,Y_N)$が与えられます。
</p>

<p>
以下の条件を全て満たす $N$行 $N$列の整数行列 $A=(A_{i,j})$$(1\le i , j \le N)$が存在するか判定し、存在する場合は一つ求めてください。
</p>

<ul>

<li>
$1\le A_{i,j} \le N$$(1\le i \le N, 1\le j\le N)$
</li>

<li>
$A_{i,j}=A_{j,i}$$(1\le i\le N, 1\le j\le N)$
</li>

<li>
$A_{i,j_1}\neq A_{i,j_2}$$(1\le i\le N, 1\le j_1 < j_2 \le N)$
</li>

<li>
$A_{i,Y_i}=1$$(1\le i\le N)$
</li>

</ul>

<p>
$T$個のテストケースが与えられるので、それぞれについて答えを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le T\le 5000$
</li>

<li>
$1\le N \le 500$
</li>

<li>
全てのテストケースにおける $N^2$の総和は $500^2$以下
</li>

<li>
$1\le Y_i\le N$
</li>

<li>
入力される値は全て整数
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる。
</p>

<div>

$N$$Y_1$$Y_2$$\ldots$$Y_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
各テストケースに対する答えを順に改行区切りで出力せよ。
</p>

<p>
各テストケースについて、条件を全て満たす $A$が存在しない場合は `No`を出力せよ。
</p>

<p>
そうでない場合、条件を全て満たす $A$を以下の形式で出力せよ。
</p>

<div>

Yes
$A_{1,1}$$A_{1,2}$$\ldots$$A_{1,N}$$A_{2,1}$$A_{2,2}$$\ldots$$A_{2,N}$$\vdots$$A_{N,1}$$A_{N,2}$$\ldots$$A_{N,N}$
</div>

<p>
条件を全て満たす $A$が複数ある場合、どれを出力しても正答となる。
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
3
1 3 2
3
1 2 3
1
1
5
1 3 2 5 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Yes
1 2 3
2 3 1
3 1 2
No
Yes
1
Yes
1 2 5 4 3
2 3 1 5 4
5 1 4 3 2
4 5 3 2 1
3 4 2 1 5

</div>

<p>
$1$つ目のテストケースについて考えます。
</p>

<p>
出力例の $A$は条件を全て満たすことが確認できます。この他にも、例えば以下のような $A$を出力しても正答となります。
</p>

<div>

1 3 2
3 2 1
2 1 3

</div>

</section>

</div>

</span>

</span>

</div>
