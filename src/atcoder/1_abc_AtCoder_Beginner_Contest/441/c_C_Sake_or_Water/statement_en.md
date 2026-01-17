
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
There are $N$cups, each containing a colorless and transparent liquid.

Specifically, the $i$-th $(1\leq i\leq N)$cup contains $A_i$ml of liquid.

It is known that exactly $K$of these cups contain sake (rice wine), and the rest contain water.

However, it is not known which cups contain sake.
</p>

<p>
Takahashi can choose some (one or more) cups and drink all the liquid in them.

Find the minimum number of cups he needs to choose to ensure he drinks at least $X$ml of sake, regardless of which cups contain sake.

If such a choice is impossible, print $-1$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq K \leq N \leq 3\times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^9$
</li>

<li>
$1 \leq X \leq 3\times 10^{14}$
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

$N$$K$$X$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the minimum number of cups Takahashi needs to choose to satisfy the condition. 
If such a choice is impossible, print $-1$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 2 5
10 6 8

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
Consider the case where Takahashi chooses the first and third cups and drinks them.
</p>

<p>
Two out of the three cups contain sake, so the following three cases are possible:
</p>

<ul>

<li>
If the first and second cups contain sake
</li>

</ul>

<p>
He drinks $10$ml of sake and $8$ml of water.
</p>

<ul>

<li>
If the first and third cups contain sake
</li>

</ul>

<p>
He drinks $18$ml of sake.
</p>

<ul>

<li>
If the second and third cups contain sake
</li>

</ul>

<p>
He drinks $8$ml of sake and $10$ml of water.
</p>

<p>
Thus, in all cases, he can drink at least $5$ml of sake.

On the other hand, it is impossible to satisfy the condition by choosing only one cup without knowing which cups contain sake.  
</p>

<p>
Therefore, print $2$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2 1 8
6 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1

</div>

<p>
If the first cup contained sake, it is impossible to drink $8$ml or more of sake no matter which cups are chosen.

Therefore, print $-1$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5 3 3000000000
1000000000 1000000000 1000000000 1000000000 1000000000

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
