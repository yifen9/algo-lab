
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
You are given integers $L, K$and a length-$N$non-negative integer sequence $A = (A_1, A_2, \ldots, A_N)$.
Here, $2K < L$and $0 \leq A_1 < A_2 < \cdots < A_N < L$are guaranteed.
</p>

<p>
Consider a circle with circumference $L$.
Take an arbitrary point on this circle as the reference point, and call the point reached by traveling clockwise distance $x$along the circumference from there the point with coordinate $x$.
Also, for each $i$($1 \leq i \leq N$), consider the chord connecting the point with coordinate $A_i$and the point with coordinate $A_i + K$, and call this chord $i$.
</p>

<p>
For a set of chords $s$, the 
<strong>
score
</strong>
is determined by the following procedure:
</p>

<ul>

<li>
Draw all chords contained in $s$. The drawn chords divide the circle into several regions; color them with white and black.
First, color the region containing the center of the circle white, and color the remaining regions so that adjacent regions (connected by a line segment of positive length) have different colors.
It can be proved that such a coloring method always exists uniquely.
The score is the number of regions colored black.
</li>

</ul>

<p>
There are $2^N$possible sets for $s$.
Find the sum, modulo $998244353$, of scores for all of these.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq K$
</li>

<li>
$2K < L \leq 10^9$
</li>

<li>
$1 \leq N \leq 250000$
</li>

<li>
$0 \leq A_1 < A_2 < \cdots < A_N < L$
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

$L$$K$$N$$A_1$$A_2$$\ldots$$A_N$
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

5 2 2
0 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4

</div>

<ul>

<li>
When no chords are chosen, the score is $0$.
</li>

<li>
When chord $1$is chosen, the score is $1$.
</li>

<li>
When chord $2$is chosen, the score is $1$.
</li>

<li>
When chords $1, 2$are chosen, the score is $2$.
</li>

</ul>

<p>
Therefore, the answer is $4$, which is the sum of these.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 1 1
2

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

5 2 5
0 1 2 3 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

80

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

7 3 3
0 2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

12

</div>

</section>

</div>

</span>

</span>

</div>
