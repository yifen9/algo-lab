
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
You are given a sequence of positive integers $A=(A_1,A_2,\ldots,A_N)$of length $N$, and you will perform $Q$operations on it. For $1\leq q\leq Q$, the $q$-th operation is given as positive integers $i_q, x_q$(where $1\leq i_q\leq N$), and it adds $x_q$to $A_{i_q}$.
</p>

<p>
Your goal is to appropriately determine the initial state of $A$so that the following condition holds at any point in time (that is, in the initial state and immediately after each operation).
</p>

<ul>

<li>
$0<A_1 < A_2 < \cdots < A_N$holds.
</li>

</ul>

<p>
When achieving this goal, find the minimum possible sum of elements in the initial state of $A$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\leq N\leq 2\times 10^5$
</li>

<li>
$1\leq Q\leq 2\times 10^5$
</li>

<li>
$1\leq i_q\leq N$
</li>

<li>
$1\leq x_q\leq 10^5$
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

$N$$Q$$i_1$$x_1$$\vdots$$i_Q$$x_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the minimum possible sum of elements in the initial state of $A$when achieving the goal.
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
1 2
2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

22

</div>

<p>
Suppose the initial state of $A$is $A=(1,4,8,9)$. Then,
</p>

<ul>

<li>
$A$immediately after the $1$-st operation: $A=(3,4,8,9)$
</li>

<li>
$A$immediately after the $2$-nd operation: $A=(3,7,8,9)$
</li>

</ul>

<p>
and it can be verified that $A$satisfies the condition at any point in time.
</p>

<p>
In this case, the sum of elements in the initial state of $A$is $\displaystyle \sum_{i=1}^NA_i=1+4+8+9=22$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 2
2 3
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

16

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

100000 1
1 100000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

14999950000

</div>

</section>

</div>

</span>

</span>

</div>
