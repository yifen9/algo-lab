
<div>

<span>

<span>

<p>
配点 : $625$点
</p>

<div>

<section>

### **問題文**

<p>
$N$個の集合 $S_1, \ldots,S_N$があります。最初、全ての集合は空集合です。
</p>

<p>
以下の形式のクエリが $Q$個与えられるので順に処理してください。
</p>

<ul>

<li>
タイプ $1$：`1 L R x`の形式で与えられる。$L \leq i \leq R$を満たす各 $S_i$に対し、$x$を追加する。
</li>

<li>
タイプ $2$：`2 L R x`の形式で与えられる。$L \leq i \leq R$を満たす各 $S_i$に対し、$x$を削除する。
</li>

<li>
タイプ $3$：`3 L R`の形式で与えられる。$L \leq i \leq R$を満たす $S_i$のうちの、要素数の最大値と、それを達成する集合の個数を求める。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N \leq 3\times 10^5$
</li>

<li>
$1\leq Q \leq 3\times 10^5$
</li>

<li>
各クエリにおいて、$1 \leq L \leq R \leq N$
</li>

<li>
タイプ $1,2$のクエリにおいて、$1 \leq x \leq 60$
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

$N$$Q$$\mathrm{query}_1$$\vdots$$\mathrm{query}_Q$
</div>

<p>
ただし、$\mathrm{query}_i$は $i$番目のクエリを表し、それぞれ問題文中に示した以下の形式で与えられる。
</p>

<div>

$1$$L$$R$$x$
</div>

<div>

$2$$L$$R$$x$
</div>

<div>

$3$$L$$R$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
タイプ $3$のクエリの個数を $q$として $q$行出力せよ。

$i$行目には、$i$個目のタイプ $3$のクエリにおいて、要素数の最大値を $x$、それを達成する集合の個数を $y$として、$x,y$を空白区切りで出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 7
1 1 2 10
1 2 4 20
3 1 3
2 1 2 20
1 2 3 10
3 1 2
3 1 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2 1
1 2
2 1

</div>

<ul>

<li>
最初 $(S_1,S_2,S_3,S_4)=(\lbrace\rbrace,\lbrace\rbrace,\lbrace\rbrace,\lbrace\rbrace)$です。
</li>

<li>
$1$番目のクエリにより $S_1,S_2$に $10$が追加され、$(S_1,S_2,S_3,S_4)=(\lbrace 10\rbrace,\lbrace 10\rbrace,\lbrace\rbrace,\lbrace\rbrace)$となります。
</li>

<li>
$2$番目のクエリにより $S_2,S_3,S_4$に $20$が追加され、$(S_1,S_2,S_3,S_4)=(\lbrace 10\rbrace,\lbrace 10,20\rbrace,\lbrace 20\rbrace,\lbrace 20\rbrace)$となります。
</li>

<li>
$3$番目のクエリにおいて、$S_1,S_2,S_3$のうち要素数が最大となるのは $S_2$の $2$個であるため、`2 1`を出力します。
</li>

<li>
$4$番目のクエリにより $S_1,S_2$から $20$が削除され、$(S_1,S_2,S_3,S_4)=(\lbrace 10\rbrace,\lbrace 10\rbrace,\lbrace 20\rbrace,\lbrace 20\rbrace)$となります。
</li>

<li>
$5$番目のクエリにより $S_2,S_3$に $10$が追加され、$(S_1,S_2,S_3,S_4)=(\lbrace 10\rbrace,\lbrace 10\rbrace,\lbrace 10,20\rbrace,\lbrace 20\rbrace)$となります。
</li>

<li>
$6$番目のクエリにおいて、$S_1,S_2$のうち要素数が最大となるのは $S_1,S_2$の $1$個であるため、`1 2`を出力します。
</li>

<li>
$7$番目のクエリにおいて、$S_1,S_2,S_3,S_4$のうち要素数が最大となるのは $S_3$の $2$個であるため、`2 1`を出力します。
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
