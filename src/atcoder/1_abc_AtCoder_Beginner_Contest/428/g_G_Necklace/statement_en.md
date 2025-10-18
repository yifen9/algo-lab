
<div>

<span>

<span>

<p>
Score : $625$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$types of jewels numbered from $1$to $N$. You have an infinite number of jewels of all types. Jewels of the same type are indistinguishable.

Also, there is an integer $U$that is $2$or greater. The beauty of each jewel is represented by an integer value between $2$and $U$, inclusive, and the beauty of jewel $i$is $b_i$.  
</p>

<p>
For each integer $x$satisfying $2 \leq x \leq U$, let $f(x)$be the answer to the following problem:
</p>

<blockquote>

<p>
You will arrange some jewels in a circular pattern to make a necklace.

Find the number, modulo $998244353$, of necklaces such that the product of the beauties of the jewels used equals $x$.

Here, two necklaces are considered the same and counted only once if they match after rotation. However, two necklaces are counted separately if they do not match just by rotation, even if they match after flipping upside down and rotating. For example, consider the following: 
</p>

<ul>

<li>
Necklace A: A necklace formed by arranging jewels $1$, $2$, $3$in this order clockwise.
</li>

<li>
Necklace B: A necklace formed by arranging jewels $2$, $3$, $1$in this order clockwise.
</li>

<li>
Necklace C: A necklace formed by arranging jewels $1$, $3$, $2$in this order clockwise.
</li>

</ul>

<p>
Here, necklaces A and B are considered the same and counted only once, but necklaces A and C are counted separately.
</p>

</blockquote>

<p>
Compute $f(2), f(3), \dots, f(U)$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 5 \times 10^5$
</li>

<li>
$2 \leq U \leq 5 \times 10^5$
</li>

<li>
$2 \leq b_i \leq U$
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

$N$$U$$b_1$$b_2$$\dots$$b_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $f(2), f(3), \dots, f(U)$separated by spaces in one line.
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
2 2 3 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2 1 4 0 2

</div>

<p>
For example, when $x=4$, the following four necklaces satisfy the condition:
</p>

<ul>

<li>
A necklace formed by arranging jewels $1$, $1$in this order clockwise.
</li>

<li>
A necklace formed by arranging jewels $1$, $2$in this order clockwise.
</li>

<li>
A necklace formed by arranging jewels $2$, $2$in this order clockwise.
</li>

<li>
A necklace formed by arranging jewel $4$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 16
2 2 2 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

4 0 10 0 0 0 24 0 0 0 0 0 0 0 70

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

14 12
10 2 2 3 8 7 11 6 12 4 9 5 3 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

3 2 7 1 7 1 15 4 4 1 24

</div>

</section>

</div>

</span>

</span>

</div>
