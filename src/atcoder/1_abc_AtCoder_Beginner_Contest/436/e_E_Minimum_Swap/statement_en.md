
<div>

<span>

<span>

<p>
Score : $475$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence $P=(P _ 1,P _ 2,\ldots,P _ N)$that is a permutation of $(1,2,\ldots,N)$.
Here, it is guaranteed that $P$is not equal to $(1,2,\ldots,N)$.
</p>

<p>
You want to perform the following operation zero or more times to make $P$match the sequence $(1,2,\ldots,N)$:
</p>

<ul>

<li>
Choose a pair of integers $(i,j)$satisfying $1\le i\lt j\le N$. Swap the values of $P _ i$and $P _ j$.
</li>

</ul>

<p>
Let $K$be the minimum number of operations required to make $P$match the sequence $(1,2,\ldots,N)$.
</p>

<p>
Find the number of operations that can be 
<strong>
the first operation
</strong>
in a sequence of operations that makes $P$match the sequence $(1,2,\ldots,N)$in $K$operations.
Two operations are distinguished if and only if the chosen pairs of integers $(i,j)$are different.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\le N\le3\times10 ^ 5$
</li>

<li>
$1\le P _ i\le N\ (1\le i\le N)$
</li>

<li>
$P _ i\ne P _ j\ (1\le i\lt j\le N)$
</li>

<li>
There exists $1\le i\le N$such that $i\ne P _ i$.
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

$N$$P _ 1$$P _ 2$$\ldots$$P _ N$
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

5
3 1 4 2 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

6

</div>

<p>
For example, the goal can be achieved in three operations as follows:
</p>

<ul>

<li>
Choose $(i,j)=(1,2)$. $P$becomes $(1,3,4,2,5)$.
</li>

<li>
Choose $(i,j)=(2,4)$. $P$becomes $(1,2,4,3,5)$.
</li>

<li>
Choose $(i,j)=(3,4)$. $P$becomes $(1,2,3,4,5)$.
</li>

</ul>

<p>
The goal cannot be achieved in two or fewer operations, so $K=3$.
</p>

<p>
As explained above, choosing $(1,2)$for the first operation allows the goal to be achieved in three operations.
Additionally, if one of $(1,3),(1,4),(2,3),(2,4),(3,4)$is chosen for the first operation, then by performing the next two operations appropriately, $P$can be made equal to $(1,2,3,4,5)$.
</p>

<p>
Therefore, print `6`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2
2 1

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

20
15 5 13 17 9 11 20 4 14 16 6 3 8 19 12 7 10 18 2 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

77

</div>

</section>

</div>

</span>

</span>

</div>
