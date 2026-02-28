
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a string $S$consisting of the three characters `A`, `B`, and `C`.
</p>

<p>
Define an operation as follows:
</p>

<blockquote>

<p>
Choose a tuple $(i, j, k)$satisfying $1 \le i \lt j \lt k \le |S|$, $S_i =$`A`, $S_j =$`B`, and $S_k =$`C`, and remove the $i$-th, $j$-th, and $k$-th characters from $S$. The remaining characters are packed to the left in their original order.
</p>

</blockquote>

<p>
Find the maximum number of times the operation can be performed on string $S$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le |S| \le 10^{6}$
</li>

<li>
$S$is a string consisting of `A`, `B`, and `C`.
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

$S$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

ABACBCC

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2

</div>

<p>
The operation can be performed twice as follows:
</p>

<ul>

<li>

<p>
For `ABACBCC`, perform the operation with $(i, j, k) = (1, 2, 7)$. The remaining string is `ACBC`.
</p>

</li>

<li>

<p>
For `ACBC`, perform the operation with $(i, j, k) = (1, 3, 4)$. The remaining string is `C`.
</p>

</li>

</ul>

<p>
The operation cannot be performed three or more times, so the answer is $2$. Thus, output $2$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

CBACBB

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

BBBAAABCBCBAACBBCAAC

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

5

</div>

</section>

</div>

</span>

</span>

</div>
