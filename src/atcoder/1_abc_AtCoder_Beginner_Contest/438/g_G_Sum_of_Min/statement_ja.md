
<div>

<span>

<span>

<p>
配点 : $575$点
</p>

<div>

<section>

### **問題文**

<p>
整数 $N,M,K$と長さ $N$の整数列 $A=(A_0,A_1,\ldots,A_{N-1})$、長さ $M$の整数列 $B=(B_0,B_1,\ldots,B_{M-1})$が与えられます。添字が $0$から始まることに注意してください。
</p>

<p>
$\displaystyle\sum_{i=0}^{K-1} \min(A_{i\bmod N}, B_{i \bmod M}) $を $998244353$で割ったあまりを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N,M\le 2\times 10^5$
</li>

<li>
$1\le K\le 10^{18}$
</li>

<li>
$1\le A_i,B_i\le 10^9$
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

$N$$M$$K$$A_0$$A_1$$\ldots$$A_{N-1}$$B_0$$B_1$$\ldots$$B_{M-1}$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$\displaystyle\sum_{i=0}^{K-1} \min(A_{i\bmod N}, B_{i \bmod M}) $を $998244353$で割ったあまりを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3 2 5
3 1 4
1 5

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

7

</div>

<p>
求める値は $\min(3,1)+\min(1,5)+\min(4,1)+\min(3,5)+\min(1,1)=7$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4 4 27
6 1 10 42
87 6 21 33

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

317

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

5 7 583272014892537201
763832259 547096173 408327452 685495693 212251318
850800766 845647066 240229336 648345577 691868483 740301913 740485849

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

931208848

</div>

<p>
$998244353$で割ったあまりを求めてください。
</p>

</section>

</div>

</span>

</span>

</div>
