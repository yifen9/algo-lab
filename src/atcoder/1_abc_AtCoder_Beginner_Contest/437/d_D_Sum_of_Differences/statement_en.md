
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
You are given a length-$N$sequence of positive integers $A = (A_1, A_2, \dots, A_N)$and a length-$M$sequence of positive integers $B = (B_1, B_2, \dots, B_M)$.
</p>

<p>
Find the value of $\displaystyle \sum_{i=1}^{N} \sum_{j=1}^{M} |A_i - B_j|$, modulo $998244353$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N,M \leq 3 \times 10^5$
</li>

<li>
$1 \leq A_i, B_j < 998244353$
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

$N$$M$$A_1$$A_2$$\cdots$$A_N$$B_1$$B_2$$\cdots$$B_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer in one line.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 2
1 6 9 2
3 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

26

</div>

<p>
The answer is $|1-3| + |1-1| + |6-3| + |6-1| + |9-3| + |9-1| + |2-3| + |2-1| = 2+0+3+5+6+8+1+1 = 26$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

8 8
185991676 311812083 311812083 84357963 185991676 185991676 724020528 369175631
455049197 387671868 4361724 724020528 724020528 455049197 455049197 724020528

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

529117255

</div>

</section>

</div>

</span>

</span>

</div>
