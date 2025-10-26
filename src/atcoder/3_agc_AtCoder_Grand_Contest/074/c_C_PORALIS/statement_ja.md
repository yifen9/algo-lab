
<div>

<span>

<span>

<p>
配点 : $900$点
</p>

<div>

<section>

### **問題文**

<p>
正整数 $N$が与えられます。

以下の条件をすべて満たすような非負整数列 $P=(P_1, P_2, \dots,P_N), A=(A_1, A_2, \dots,A_N)$を $1$つ出力してください。
</p>

<ul>

<li>
$0 \leq P_i < 2^{30}~(1 \leq i \leq N)$
</li>

<li>
$0 \leq A_i < 2^{30}~(1 \leq i \leq N)$
</li>

<li>
$(P_1~\mathrm{OR}~A_i, P_2~\mathrm{OR}~A_i, \dots, P_N~\mathrm{OR}~A_i)$の最長狭義単調増加部分列の長さは $i$である。$(1 \leq i \leq N)$
<ul>

<li>
$\mathrm{OR}$はビット単位 $\mathrm{OR}$演算を表します。
</li>

</ul>

</li>

</ul>

<p>
この問題の制約下で、条件を満たす $P, A$が $1$つ以上存在することが証明できます。
</p>

<p>
$1$つの入力につき、$T$個のテストケースを解いてください。
</p>

<details>

<summary>
ビット単位 $\mathrm{OR}$演算とは
    
</summary>

<p>
非負整数 $A, B$のビット単位 $\mathrm{OR}$、$A\ \mathrm{OR}\ B$は以下のように定義されます。
        
</p>

<ul>

<li>
$A\ \mathrm{OR}\ B$を二進表記した際の $2^k$($k \geq 0$) の位の数は、$A, B$を二進表記した際の $2^k$の位の数のうち少なくとも片方が $1$であれば $1$、そうでなければ $0$である。
</li>

</ul>
例えば、$3\ \mathrm{OR}\ 5 = 7$となります (二進表記すると: $011\ \mathrm{OR}\ 101 = 111$)。


<p>

</p>

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq T$
</li>

<li>
$1 \leq N \leq 1024$
</li>

<li>
$1$つの入力に含まれるテストケースについて、$N$の総和は $200000$以下  
</li>

<li>
$1$つの入力に含まれるテストケースについて、$N^2$の総和は $1024^2$以下  
</li>

<li>
入力はすべて整数
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
各ケースは以下の形式で与えられる。
</p>

<div>

$N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$t$番目に $\mathrm{case}_t$に対する答えを出力せよ。  
</p>

<p>
各ケースについて、以下の形式に従って答えを出力せよ。
</p>

<div>

$P_1$$P_2$$\ldots$$P_N$$A_1$$A_2$$\ldots$$A_N$
</div>

<p>
答えが複数存在する場合、どれを出力しても正解となる。
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
3
8
1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3 14 5
13 2 10
6 902 909 186 684 219 471 248
1023 249 64 0 264 768 778 794
2025
1026

</div>

<p>
$1$番目のテストケースについて、出力例は $P = (3, 14, 5), A = (13, 2, 10)$です。
</p>

<ul>

<li>
$(3~\mathrm{OR}~13, 14~\mathrm{OR}~13, 5~\mathrm{OR}~13) = (15, 15, 13)$の最長狭義単調増加部分列の $1$つは $(13)$であり、その長さは $1$です。
</li>

<li>
$(3~\mathrm{OR}~2, 14~\mathrm{OR}~2, 5~\mathrm{OR}~2) = (3, 14, 7)$の最長狭義単調増加部分列の $1$つは $(3, 7)$であり、その長さは $2$です。
</li>

<li>
$(3~\mathrm{OR}~10, 14~\mathrm{OR}~10, 5~\mathrm{OR}~10) = (11, 14, 15)$の最長狭義単調増加部分列の $1$つは $(11, 14, 15)$であり、その長さは $3$です。
</li>

</ul>

<p>
上記より、$P = (3, 14, 5), A = (13, 2, 10)$は条件を満たすことが確認できます。
</p>

</section>

</div>

</span>

</span>

</div>
