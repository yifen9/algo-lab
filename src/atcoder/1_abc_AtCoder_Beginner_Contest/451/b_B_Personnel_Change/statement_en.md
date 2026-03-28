
<div>

<span>

<span>

<p>
Score : $200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
The company where Takahashi works has $N$employees, each assigned an employee number from $1, 2, \dots, N$.
There are $M$departments in the company, called departments $1, 2, \dots, M$.
</p>

<p>
Employee $i$belongs to department $A_i$this term and will belong to department $B_i$next term.
</p>

<p>
For each of departments $1, 2, \dots, M$, find the number of members next term minus the number of members this term.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 100$
</li>

<li>
$1 \leq M \leq 100$
</li>

<li>
$1 \leq A_i \leq M$
</li>

<li>
$1 \leq B_i \leq M$
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

$N$$M$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_N$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $M$lines. The $j$-th line should contain the answer for department $j$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 4
1 2
2 1
3 1
2 2
2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
-1
-1
1

</div>

<ul>

<li>
For department $1$: this term, one employee (employee number $1$) belongs; next term, two employees (employee numbers $2, 3$) belong.
</li>

<li>
For department $2$: this term, three employees (employee numbers $2, 4, 5$) belong; next term, two employees (employee numbers $1, 4$) belong.
</li>

<li>
For department $3$: this term, one employee (employee number $3$) belongs; next term, no one belongs.
</li>

<li>
For department $4$: this term, no one belongs; next term, one employee (employee number $5$) belongs.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 5
3 2
3 4
1 2
2 2
4 4
3 1
3 4
4 2
3 3
3 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0
4
-5
1
0

</div>

</section>

</div>

</span>

</span>

</div>
