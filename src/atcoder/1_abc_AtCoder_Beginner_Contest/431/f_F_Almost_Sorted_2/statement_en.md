
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence $A=(A_1,A_2,\ldots,A_N)$of length $N$and a positive integer $D$.
</p>

<p>
Find the number, modulo $998244353$, of integer sequences $B=(B_1, B_2, \ldots, B_N)$that can be obtained by rearranging $A$and satisfy the following condition:
</p>

<ul>

<li>
$B_{i+1}\geq B_i-D$holds for all $i\ (1\leq i\leq N-1)$.
</li>

</ul>

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
$1\leq D\leq 10^6$
</li>

<li>
$1\leq A_i\leq 10^6$
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

$N$$D$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 1
5 2 1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3

</div>

<p>
The integer sequences satisfying the condition are $(1,2,2,5),(2,1,2,5),(2,2,1,5)$, which are three sequences.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 10
20 40 60 80 100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

15 12345
18270 31252 27543 31406 22271 13402 12279 25697 18349 27615 39360 22790 32581 23990 36154

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

858152905

</div>

</section>

</div>

</span>

</span>

</div>
