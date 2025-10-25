
<div>

<span>

<span>

<p>
Score : $625$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given integers $N,M,A,B,X,R$.
</p>

<p>
Find the remainder when $\displaystyle \sum_{k=0}^{N-1} X^{(Ak+B) \bmod M}$is divided by $R$.
</p>

<p>
You are given $T$test cases, so find the answer for each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le T\le 100$
</li>

<li>
$1\le N,M,R\le 10^9$
</li>

<li>
$0\le A,B < M$
</li>

<li>
$1\le X < R$
</li>

<li>
All input values are integers.
</li>

</ul>

</section>

</div>

---

<div>

<div>

<section>

### **Input**

<p>
The input is given from Standard Input in the following format:
</p>

<div>

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case $\text{case}_i$is given in the following format:
</p>

<div>

$N$$M$$A$$B$$X$$R$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $T$lines.
</p>

<p>
On the $i$-th line, print the remainder when $\displaystyle \sum_{k=0}^{N-1} X^{(Ak+B) \bmod M}$is divided by $R$for the $i$-th test case.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
4 5 2 1 2 1000000000
777 429 33 58 1 1000000000
20251025 429429 777 1025 575757 998244353

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

15
777
445271630

</div>

<p>
Consider the first test case.
</p>

<ul>

<li>
When $k=0$: $\displaystyle X^{(Ak+B) \bmod M}=2^{(2\times 0+1) \bmod 5}=2^1=2$.
</li>

<li>
When $k=1$: $\displaystyle X^{(Ak+B) \bmod M}=2^{(2\times 1+1) \bmod 5}=2^3=8$.
</li>

<li>
When $k=2$: $\displaystyle X^{(Ak+B) \bmod M}=2^{(2\times 2+1) \bmod 5}=2^0=1$.
</li>

<li>
When $k=3$: $\displaystyle X^{(Ak+B) \bmod M}=2^{(2\times 3+1) \bmod 5}=2^2=4$.
</li>

</ul>

<p>
From the above, the desired value is the remainder when $2+8+1+4$is divided by $1000000000$, which is $15$. Therefore, print $15$on the $1$st line.
</p>

</section>

</div>

</span>

</span>

</div>
