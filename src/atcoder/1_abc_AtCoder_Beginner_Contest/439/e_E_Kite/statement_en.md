
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<p>
Happy New Year! When it comes to outdoor play on New Year's, it's kite flying!
</p>

</blockquote>

<p>
$N$people numbered $1$to $N$are trying to fly kites by the riverbank.

The river facing the riverbank flows in a straight line, so from now on, we consider a two-dimensional coordinate system where the $x$-axis is the direction of the river and the $y$-axis is the height direction.

Person $i$is standing at point $(A_i, 0)$and trying to fly a kite at point $(B_i, 1)$.

However, to avoid collisions of people and kites, and to avoid kite strings getting tangled, persons $i$and $j$($i \neq j$) cannot fly kites at the same time if the following condition is satisfied:  
</p>

<ul>

<li>
The "line segment connecting $(A_i, 0)$and $(B_i, 1)$" and the "line segment connecting $(A_j, 0)$and $(B_j, 1)$" have an intersection point. (This includes the case where the endpoints of the line segments touch each other.)
</li>

</ul>

<p>
What is the maximum number of people who can fly kites at the same time while respecting the above constraint?
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 2\times 10^5$
</li>

<li>
$0 \leq A_i \leq 10^9$
</li>

<li>
$0 \leq B_i \leq 10^9$
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

$N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_N$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the maximum number of people who can fly kites at the same time.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
3 5
1 4
2 6

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
Persons $1$and $2$, as well as persons $2$and $3$, can fly kites at the same time, but persons $1$and $3$cannot fly kites at the same time.

Therefore, two people, if chosen appropriately, can fly kites at the same time, while it is impossible for three people to fly kites at the same time. Thus, the answer is $2$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
1 2
1 3
1 4
1 5
1 6

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

10
440423913 766294629
725560240 59187619
965580535 585990756
550925213 623321125
549392044 122410708
21524934 690874816
529970099 244587368
757265587 736247509
576136367 993115118
219853537 21553211

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

4

</div>

</section>

</div>

</span>

</span>

</div>
