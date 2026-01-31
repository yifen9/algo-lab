
<div>

<span>

<span>

<p>
Score : $575$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given integers $N,M,A,B$.
</p>

<p>
Define an integer sequence $X=(X_0,X_1,\ldots,X_{N-1})$as $\displaystyle X_k = (Ak+B) \bmod M$.
</p>

<p>
Find the number of integers $k$satisfying $0 \le k < N$and $X_k > k$.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le T\le 3\times 10^5$
</li>

<li>
$1\le N \le M\le 10^9$
</li>

<li>
$0\le A,B < M$
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
Each test case is given in the following format:
</p>

<div>

$N$$M$$A$$B$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for the test cases in order, separated by newlines.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4
4 6 4 3
7 7 3 1
10 46 0 12
443 2026 131 210

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
3
10
395

</div>

<p>
Consider the first test case.
</p>

<ul>

<li>
When $k=0$: $X_0=(4\times 0+3)\bmod 6=3$, so $X_k>k$holds.
</li>

<li>
When $k=1$: $X_1=(4\times 1+3)\bmod 6=1$, so $X_k>k$does not hold.
</li>

<li>
When $k=2$: $X_2=(4\times 2+3)\bmod 6=5$, so $X_k>k$holds.
</li>

<li>
When $k=3$: $X_3=(4\times 3+3)\bmod 6=3$, so $X_k>k$does not hold.
</li>

</ul>

<p>
From the above, the integers $k$satisfying $0 \le k < 4$and $X_k>k$are $k=0,2$, which is two integers. Thus, output $2$on the first line.
</p>

</section>

</div>

</span>

</span>

</div>
