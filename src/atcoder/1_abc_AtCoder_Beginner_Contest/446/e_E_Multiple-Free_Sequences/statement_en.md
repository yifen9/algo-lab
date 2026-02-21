
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Among integer pairs $(x, y)$satisfying $0 \leq x,y \leq M-1$, how many are there such that the infinite sequence $(s_1, s_2, \dots)$defined by the following recurrence relation contains no multiples of $M$?
</p>

<ul>

<li>
$s_1 = x$
</li>

<li>
$s_2 = y$
</li>

<li>
$s_n = A s_{n-1} + B s_{n-2}$($n \geq 3$)
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq M \leq 1000$
</li>

<li>
$0 \leq A, B \leq M-1$
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

$M$$A$$B$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer on one line.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

7

</div>

<p>
The integer pairs satisfying the condition in the problem statement are $(x,y) = (1,1), (1,3), (2,1), (2,2), (2,3), (3,1), (3,3)$, for a total of seven pairs.
</p>

<p>
For example, when $(x,y) = (2,1)$, the corresponding sequence is $(2,1,5,7,17,31,65,127,\dots)$. This sequence contains no multiples of $4$. Thus, $(x,y) = (2,1)$satisfies the condition in the problem statement.
</p>

<p>
On the other hand, when $(x,y) = (3,2)$, the corresponding sequence is $(3,2,8,12,28,52,108,212,\dots)$. The third term of this sequence is $8$, which is a multiple of $4$. Thus, $(x,y) = (3,2)$does not satisfy the condition in the problem statement.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

446 1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

<p>
No integer pairs satisfy the condition in the problem statement.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

1000 784 385

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

995373

</div>

</section>

</div>

</span>

</span>

</div>
