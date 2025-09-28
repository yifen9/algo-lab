
<div>

<span>

<span>

<p>
Score : $1700$points
</p>

<div>

<section>

### **Problem Statement**

<p>
In this world, there are $K$types of gems numbered from $1$to $K(=4)$.
The value per unit size of a gem of type $i$is $W_i$.
</p>

<p>
Snuke has $N$gems.
The $i$-th gem is of type $A_i$and has size $B_i$.
Also, Snuke has $N$boxes, where the $i$-th box has size $i$.
</p>

<p>
Snuke will now put one gem in each box.
When a gem's size is larger than the box, the gem is cut to fit in the box.
That is, when gem $i$is put in box $j$, its value becomes $W_{A_i} \times \min(B_i, j)$.
</p>

<p>
Find the maximum possible sum of gem values.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>

<span>
$K = 4$
</span>

</li>

<li>
$1 \leq W_1 < W_2 < \cdots < W_K \leq 10^6$
</li>

<li>
$1 \leq N \leq 250000$
</li>

<li>
$1 \leq A_i \leq K$
</li>

<li>
$1 \leq B_i \leq N$
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

$N$$K$$W_1$$W_2$$\ldots$$W_K$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_N$$B_N$
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

3 4
1 2 3 4
4 2
1 3
3 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

15

</div>

<p>
If gems $1, 2, 3$are put in boxes $3, 1, 2$, respectively, the sum of values is $4 \times \min(2, 3) + 1 \times \min(3, 1) + 3 \times \min(2, 2) = 15$, which is maximum.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 4
1 2 3 4
3 1
2 2
1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

10

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

6 4
1 3 8 10
2 2
1 4
2 2
3 1
3 4
4 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

86

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

15 4
239277 249169 419371 744281
2 14
1 4
1 11
4 12
1 7
2 12
3 15
2 5
3 4
1 8
3 2
4 1
1 15
3 5
2 8

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

39858078

</div>

</section>

</div>

</span>

</span>

</div>
