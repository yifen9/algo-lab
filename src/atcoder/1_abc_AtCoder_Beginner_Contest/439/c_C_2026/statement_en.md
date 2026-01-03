
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
A positive integer $n$is called a 
<strong>
good integer
</strong>
when it satisfies the following condition:
</p>

<ul>

<li>
There exists exactly one pair of integers $(x,y)$that satisfies $0 \lt x \lt y$and $x^2+y^2=n$.
</li>

</ul>

<p>
For example, when $n=2026$, it can be verified that $(x,y)=(1,45)$is the only pair of integers that satisfies $0 \lt x \lt y$and $x^2+y^2=n$. Thus, $2026$is a good integer.
</p>

<p>
You are given a positive integer $N$. Enumerate all good integers not exceeding $N$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 10^7$
</li>

<li>
$N$is an integer.
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
Let there be $k$good integers not exceeding $N$, and let $(a_1, a_2, \dots, a_k)$be the sequence of these integers in ascending order. Output the answer in the following format. (If $k=0$, output the second line as an empty line.)
</p>

<div>

$k$$a_1$$a_2$$\dots$$a_k$
</div>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
5 10

</div>

<p>
$(x,y)=(1,2)$is the only pair of integers that satisfies $0 \lt x \lt y$and $x^2+y^2=5$, so $5$is a good integer.

$(x,y)=(1,3)$is the only pair of integers that satisfies $0 \lt x \lt y$and $x^2+y^2=10$, so $10$is a good integer.

These are the only two good integers not exceeding $N$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1

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

50

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

14
5 10 13 17 20 25 26 29 34 37 40 41 45 50

</div>

</section>

</div>

</span>

</span>

</div>
