
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$dominoes standing in a row on a number line. The $i$-th domino is standing at coordinate $i$and has height $A_i$.
</p>

<p>
When the $i$-th domino falls to the right, all dominoes in the range between coordinates $i$and $i+A_i-1$, inclusive, fall to the right.
</p>

<p>
How many dominoes will fall in total when the first domino falls to the right?
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N \leq 5\times 10^5$
</li>

<li>
$1\leq A_i \leq N$
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

$N$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the number of dominoes that fall when the first domino falls to the right.
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
3 1 4 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4

</div>

<p>
When the first domino falls to the right, the second and third dominoes also fall to the right. When the third domino falls to the right, the fourth domino also falls.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

9
1 4 1 4 2 1 3 5 6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

<p>
When the first domino falls to the right, no other dominoes will fall.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10
5 4 3 2 1 1 2 3 4 5

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
