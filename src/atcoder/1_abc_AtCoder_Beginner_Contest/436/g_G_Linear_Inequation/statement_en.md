
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a length-$N$sequence of positive integers $A=(A _ 1,A _ 2,\ldots,A _ N)$and a positive integer $M$. 
</p>

<p>
Find the number of length-$N$sequences of non-negative integers $x=(x _ 1,x _ 2,\ldots,x _ N)$that satisfy the following condition:
</p>

<ul>

<li>
$\displaystyle\sum _ {i=1} ^ NA _ ix _ i\le M$
</li>

</ul>

<p>
The number can be very large, so find it modulo $998244353$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le100$
</li>

<li>
$1\le A _ i\le100\ (1\le i\le N)$
</li>

<li>
$1\le M\le10 ^ {18}$
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

$N$$M$$A _ 1$$A _ 2$$\ldots$$A _ N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the number, modulo $998244353$, of non-negative integer sequences that satisfy the condition.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 6
5 4 3 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

10

</div>

<p>
The sequences $x$that satisfy the condition are the following $10$: $(0,0,0,0),(0,0,0,1),(0,0,0,2),(0,0,0,3),(0,0,1,0),(0,0,1,1),(0,0,2,0),(0,1,0,0),(0,1,0,1),(1,0,0,0)$.
</p>

<p>
Thus, print `10`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6 89
4 7 5 10 7 6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

38469

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

1 1000000007
1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

1755655

</div>

<p>
There are $1000000008$sequences $x$that satisfy the condition.
</p>

<p>
Print this modulo $998244353$, which is $1755655$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

20 738894495848985641
40 58 13 24 65 11 63 29 98 75 40 77 15 50 83 85 35 46 38 37

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

31156940

</div>

</section>

</div>

</span>

</span>

</div>
