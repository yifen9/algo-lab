
<div>

<span>

<span>

<p>
配点 : $800$点
</p>

<div>

<section>

### **問題文**

<p>
`A`, `B`からなる長さ $N$の文字列 $X,Y$が与えられます．$X$の $i$文字目を $X_i$と表すことにします．
</p>

<p>
以下の操作を $0$回以上 $\left\lfloor \frac{N}{2} \right\rfloor$回以下行うことで， $X$を $Y$に一致させることができるか否かを判定してください．
</p>

<ul>

<li>
$1\leq l < r \leq N$かつ $X_l=$`A`かつ $X_r=$`B`なる整数組 $(l, r)$を選ぶ．$X$の $l$番目から $r$番目までの要素を反転する．ここで，「$X$の $l$番目から $r$番目までの要素を反転する」とは，
$X_l,X_{l+1},\ldots,X_{r-1},X_r$を $X_r,X_{r-1},\ldots,X_{l+1},X_l$に同時に置き換えることを言う．
</li>

</ul>

<p>
$X$を $Y$に一致させることが可能な場合には，そのような手順をひとつ出力してください．
</p>

<p>
$T$個のテストケースが与えられるので，それぞれについて答えを求めてください．
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq T \leq  2.5\times 10^5$
</li>

<li>
$2 \leq N \leq 5\times 10^5$
</li>

<li>
一つのテストケースに含まれる $N$の総和は $5\times 10^5$以下
</li>

<li>
$X,Y$は `A`, `B`からなる長さ $N$の文字列
</li>

<li>
入力される数値は全て整数
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる．
</p>

<div>

$N$$X$$Y$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$\mathrm{case}_1,\mathrm{case}_2,\ldots,\mathrm{case}_T$に対する答えを順に以下の形式で出力せよ．
</p>

<p>
$0$回以上 $\left\lfloor \frac{N}{2} \right\rfloor$回以下の操作で $X$を $Y$に一致させることが不可能な場合には，`No`と出力せよ．
</p>

<p>
可能な場合には，操作手順を次の形式で出力せよ．
</p>

<div>

Yes
$K$$l_1$$r_1$$l_2$$r_2$$\vdots$$l_K$$r_K$
</div>

<p>
ここで $K$は操作回数で，$l_i,r_i$は $i$回目の操作で選ぶ整数 $l,r$を表す．これらは次を満たす必要がある．
</p>

<ul>

<li>
$0 \leq K \leq \left\lfloor \frac{N}{2} \right\rfloor$
</li>

<li>
$1 \leq l_i < r_i \leq N$
</li>

</ul>

<p>
条件を満たす操作手順が複数存在する場合には，そのどれを出力しても正解と見なされる．
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
5
ABAAB
ABBAA
4
AAAA
BBBB
10
BABBAABBAA
BBBBAAABAA

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Yes
1
3 5
No
Yes
3
2 7
4 6
3 5

</div>

<p>
$1$番目のテストケースでは，$X_3=$`A`かつ $X_5=$`B`なので，$X$の $3$番目から $5$番目までの要素を反転する操作を行うことができます．この操作を行うと， $X$は `ABBAA`になり，$Y$と一致します．
</p>

<p>
$2$番目のテストケースでは，どのように操作を行っても $X$を $Y$に一致させることができません．
</p>

</section>

</div>

</span>

</span>

</div>
