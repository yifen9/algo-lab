
<div>

<span>

<span>

<p>
配点 : $200$点
</p>

<div>

<section>

### **問題文**

<p>
$N$個の駅 $1,2,\dots,N$があり、これらはこの順に西から東に一直線上に並んでいます。

AtCoder 鉄道の電車はこれら $N$個の駅を通り、西から東に走っています。

$1 \leq i \lt j \leq N$を満たす任意の $2$整数 $i,j$について、駅 $i$から電車に乗って駅 $j$で降りるのにコストが $C_{i,j}$かかります。
</p>

<p>
以下のような $3$つの整数 $a,b,c$が存在するかを判定してください。  
</p>

<ul>

<li>
$1 \leq a \lt b \lt c \leq N$
</li>

<li>
駅 $a$から電車に乗って駅 $c$で降りるときにかかるコストよりも、駅 $a$から電車に乗って駅 $b$で降り、再度、駅 $b$から電車に乗って駅 $c$で降りるときにかかるコストの総和の方が小さい。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$3 \leq N \leq 100$
</li>

<li>
$1 \leq C_{i,j} \leq 10^9$
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

$N$$C_{1,2}$$C_{1,3}$$\dots$$C_{1,N}$$C_{2,3}$$\dots$$C_{2,N}$$\vdots$$C_{N-1,N}$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
条件を満たす $3$整数 $a,b,c$が存在するならば `Yes`を、存在しないならば `No`を $1$行で出力せよ。
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
45 450
45

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Yes

</div>

<p>
$(a,b,c)$として $(1,2,3)$を選ぶと、

$C_{a,b}+C_{b,c}=C_{1,2}+C_{2,3}=45+45$

$C_{a,c}=C_{1,3}=450$

なので、条件を満たします。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4
25 40 65
30 55
25

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

No

</div>

<p>
どのように $(a,b,c)$を選んでも、条件を満たしません。
</p>

</section>

</div>

</span>

</span>

</div>
