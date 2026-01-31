
<div>

<span>

<span>

<p>
Score : $525$points
</p>

<div>

<section>

### **Problem Statement**

<p>
A positive integer $X$is called a 
<strong>
good integer
</strong>
if and only if it satisfies the following condition:
</p>

<ul>

<li>
When $X$is written in decimal notation, the ones digit, tens digit, $\ldots$form a non-increasing sequence.
<ul>

<li>
More formally, the unique non-negative integer sequence $(d_0,d_1,\ldots)$satisfying $\displaystyle X=\sum_{i=0}^{\infty} d_i10^i$$(0\le d_i < 10)$forms a non-increasing sequence.
</li>

</ul>

</li>

</ul>

<p>
For example, $112389$, $1$, and $777$are good integers, but $443$and $404$are not good integers.
</p>

<p>
You are given a positive integer $N$.
</p>

<p>
Determine whether there exists a good integer that is a multiple of $N$, and if it exists, find its minimum value.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le 3\times 10^6$
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
If there does not exist a good integer that is a multiple of $N$, output $-1$.
</p>

<p>
If it exists, output the minimum value of a good integer that is a multiple of $N$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

21

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

126

</div>

<p>
$126$is a multiple of $21$, and we have $6 \geq 2 \geq 1 \geq 0 \geq \ldots$, so it is a good integer. There does not exist a good integer less than $126$that is a multiple of $21$, so output $126$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

3

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

1089

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

9999999999999999999999

</div>

<p>
The answer may be $2^{64}$or greater.
</p>

</section>

</div>

</span>

</span>

</div>
