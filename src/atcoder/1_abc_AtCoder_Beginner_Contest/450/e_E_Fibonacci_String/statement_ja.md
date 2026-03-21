
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
文字列 $X,Y$が与えられます。文字列の列 $S_1,S_2,\dots$を以下で定義します。
</p>

<ul>

<li>
$S_1=X$
</li>

<li>
$S_2=Y$
</li>

<li>
$i\geq 3$のとき、$S_i$は $S_{i-1}$と $S_{i-2}$をこの順に連結したもの
</li>

</ul>

<p>
各 $i=1,2,\ldots,Q$について以下の問題に答えてください。
</p>

<p>
問題：整数 $L_i,R_i$と文字 $C_i$が与えられる。 $S_{10^{18}}$の $L_i$文字目から $R_i$文字目までに文字 $C_i$が何個含まれるか求めよ。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$X,Y$は英小文字からなる長さ $1$以上 $10^4$以下の文字列
</li>

<li>
$1 \leq Q \leq 10^5$
</li>

<li>
$1 \leq L_i \leq R_i \leq 10^{18}$
</li>

<li>
$C_i$は英小文字
</li>

<li>
与えられる数値は全て整数
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

$X$$Y$$Q$$L_1$$R_1$$C_1$$L_2$$R_2$$C_2$$\vdots$$L_Q$$R_Q$$C_Q$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$Q$行出力せよ。

$i$行目には  $S_{10^{18}}$の $L_i$文字目から $R_i$文字目までに文字 $C_i$が何個含まれるかを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

a
b
6
2 7 a
1 3 b
3 7 b
1 9 c
1 1000000000000000000 b
1000000000000000000 1000000000000000000 a

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3
2
3
0
618033988749894848
1

</div>

<p>
$S_3,S_4,S_5$はそれぞれ`ba`, `bab`, `babba`となります。
</p>

<p>
$S_{10^{18}}$は `babbababbabba...`であり、その $2$文字目から $7$文字目に `a`は $3$個含まれます。
</p>

</section>

</div>

</span>

</span>

</div>
