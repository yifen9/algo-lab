
<div>

<span>

<span>

<p>
Score : $1100$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Find the number, modulo $998244353$, of strings $S$of length $N$consisting of `A`, `B`, `C`such that the following value equals $K$:
</p>

<ul>

<li>
The maximum length of a (not necessarily contiguous) subsequence of $S$that does not contain `ABC`as a (not necessarily contiguous) subsequence
</li>

</ul>

<p>
You are given $T$test cases. Solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 2 \times 10^5$
</li>

<li>
$1 \le N \le 10^6$
</li>

<li>
$\max(0,N-100) \le K \le N$
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each case is given in the following format:
</p>

<div>

$N\ K$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line $(1 \le i \le T)$should contain the answer to the $i$-th test case.
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
4 3
8 6
123 100
123456 123400

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

9
462
741573397
255048895

</div>

<p>
For the first test case, for example, `ACBC`satisfies the condition. `ACBC`itself contains `ABC`as a subsequence, and `ACC`does not contain `ABC`as a subsequence, so the maximum length of a subsequence that does not contain `ABC`as a subsequence is $3$.
Other examples that satisfy the condition include `AABC`and `ABCA`.
</p>

</section>

</div>

</span>

</span>

</div>
