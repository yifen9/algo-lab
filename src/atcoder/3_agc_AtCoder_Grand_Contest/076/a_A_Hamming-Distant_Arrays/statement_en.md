
<div>

<span>

<span>

<p>
Score : $700$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer $N$.
For length-$N^2$integer sequences $a$and $b$consisting of integers between $1$and $N$(inclusive), we define their distance $d(a,b)$as follows:
</p>

<ul>

<li>
$d(a,b)=$"the number of indices $i$($1 \leq i \leq N^2$) such that $a_i \neq b_i$."
</li>

</ul>

<p>
Now, you will create $N$length-$N^2$integer sequences consisting of integers between $1$and $N$, and denote them as $x_1,x_2,\cdots,x_N$(their order also matters).
Find the number, modulo $998244353$, of instances of $(x_1,x_2,\cdots,x_N)$satisfying the following condition.
</p>

<ul>

<li>
For any length-$N^2$integer sequence $y$consisting of integers between $1$and $N$, there exists some $1 \leq i \leq N$such that $d(x_i,y) \geq N^2-N$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 50$
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

$N$
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

2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

80

</div>

<p>
For example, $(x_1,x_2)=((1,1,2,2),(1,2,1,2))$does not satisfy the condition, because if $y=(1,1,1,2)$, then $d(x_1,y)=1,d(x_2,y)=1$.
</p>

<p>
On the other hand, $(x_1,x_2)=((1,1,1,1),(2,2,2,2))$satisfies the condition.
</p>

<p>
There are $80$instances of $(x_1,x_2)$that satisfy the condition.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

597965565

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

241191911

</div>

</section>

</div>

</span>

</span>

</div>
