
<div>

<span>

<span>

<p>
配点 : $1200$点
</p>

<div>

<section>

### **問題文**

<p>
文字列 $X = X_1X_2\dots X_{|X|}$と正整数 $l,r~(1 \leq l \leq r \leq |X|)$に対して、$X_{l,r} = X_l X_{l+1}\dots X_r$とします。 
</p>

<p>
`A`, `B`からなる文字列 $S=S_1S_2\dots S_{|S|}$が与えられます。

$Q$個のクエリが与えられるので、それぞれについて以下の問いに答えてください。
</p>

<ul>

<li>
$T = S_{l,r}$とした状態から、「$T$に連続部分文字列として含まれる `AB`を $1$つ選び削除する」という操作を $0$回以上行うことによって得られる回文としてあり得る長さの最小値を求めてください。

どのように操作を行っても回文が得られない場合は `-1`を出力してください。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq |S| \leq 4 \times 10^5$
</li>

<li>
$1 \leq Q \leq 5 \times 10^4$
</li>

<li>
$1 \leq l \leq r \leq |S|$
</li>

<li>
$S$は `A`, `B`からなる文字列
</li>

<li>
$Q,l,r$は整数
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

$S$$Q$$\mathrm{Query}_1$$\mathrm{Query}_2$$\vdots$$\mathrm{Query}_Q$
</div>

<p>
$\mathrm{Query}_q$は $q$個目のクエリを表し、以下の形式で与えられる。
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
$Q$行出力せよ。$q$行目に $\mathrm{Query}_q$に対する答えを出力せよ。  
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

ABBABB
5
1 6
4 5
3 5
2 3
3 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2
0
1
2
-1

</div>

<p>
$1$個目、$2$個目、$3$個目のクエリについて、以下のように操作を行うことで、操作によって得られる回文のうち長さが最小のものが得られます。
</p>

<ul>

<li>
`ABBABB`$\rightarrow$`ABBB`$\rightarrow$`BB`
</li>

<li>
`AB`$\rightarrow$(空文字列)
</li>

<li>
`BAB`$\rightarrow$`B`
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
