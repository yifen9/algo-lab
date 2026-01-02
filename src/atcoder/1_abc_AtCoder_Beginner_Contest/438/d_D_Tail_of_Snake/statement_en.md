
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<p>
Snuke is observing a snake and is curious about which parts are the head, body, and tail.
He divided the snake into $N$blocks and evaluated the head-likeness, body-likeness, and tail-likeness of each block.
Then, he decided to find the division that maximizes the sum of the likeness values.
</p>

</blockquote>

<p>
You are given length-$N$integer sequences $A = (A_1, A_2, \ldots, A_N)$, $B = (B_1, B_2, \ldots, B_N)$, and $C = (C_1, C_2, \ldots, C_N)$.
</p>

<p>
Find the maximum possible value of $\displaystyle\sum_{i = 1}^{x} A_i + \sum_{i = x + 1}^{y} B_i + \sum_{i = y + 1}^{N} C_i$for a pair of integers $(x, y)$satisfying $1 \leq x < y < N$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3 \leq N \leq 3 \times 10^5$
</li>

<li>
$1 \leq A_i, B_i, C_i \leq 10^6$
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

$N$$A_1$$A_2$$\ldots$$A_N$$B_1$$B_2$$\ldots$$B_N$$C_1$$C_2$$\ldots$$C_N$
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

5
1 4 2 4 3
2 3 4 2 2
3 2 4 4 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

16

</div>

<p>
With $(x, y) = (2, 3)$, we have $\displaystyle\sum_{i = 1}^{x} A_i + \sum_{i = x + 1}^{y} B_i + \sum_{i = y + 1}^{N} C_i = 1 + 4 + 4 + 4 + 3 = 16$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
1 1 1
1 1 1
1 1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

3

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

6
2 10 7 7 7 11
5 7 9 10 9 12
6 6 7 10 12 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

50

</div>

</section>

</div>

</span>

</span>

</div>
