
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
A bag contains $N$balls numbered $1$to $N$. Ball $i$has the integer $A_i$written on it.

Process $Q$queries.

For each query, a sequence $B_1, B_2, \dots, B_{K}$of length $K$is given, and you should perform the following sequence of operations. Here, all $B_i$are between $1$and $N$inclusive and are distinct.
</p>

<ul>

<li>
First, remove balls $B_1$, $B_2$, $\dots$, $B_K$from the bag.
</li>

<li>
Then, output the minimum value among the integers written on the balls currently in the bag. (It is guaranteed by the constraints that the bag is not empty at this point.)
</li>

<li>
Afterwards, return all $K$removed balls to the bag.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$6 \leq N \leq 3 \times 10^5$
</li>

<li>
$1 \leq Q \leq 2 \times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^9$
</li>

<li>
$1 \leq K \leq 5$
</li>

<li>
$1 \leq B_1 \lt B_2 \lt \dots \lt B_K \leq N$
</li>

<li>
The sum of $K$over all queries is at most $4 \times 10^5$.
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
The input is given from Standard Input in the following format, where $\mathrm{query}_i$denotes the $i$-th query.
</p>

<div>

$N$$Q$$A_1$$A_2$$\dots$$A_N$$\mathrm{query}_1$$\mathrm{query}_2$$\vdots$$\mathrm{query}_Q$
</div>

<p>
Each query is given in the following format.
</p>

<div>

$K$$B_1$$B_2$$\dots$$B_K$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $i$-th line should contain the answer to the $i$-th query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

6 6
3 2 5 9 1 2
2
4 5
5
1 2 3 4 6
3
2 5 6
4
1 2 5 6
1
5
3
1 2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
1
3
5
2
1

</div>

<p>
For example, in the first query, balls $4$and $5$are removed from the bag. At this point, the following four balls remain in the bag:
</p>

<ul>

<li>
Ball $1$with $3$written on it
</li>

<li>
Ball $2$with $2$written on it
</li>

<li>
Ball $3$with $5$written on it
</li>

<li>
Ball $6$with $2$written on it
</li>

</ul>

<p>
Thus, the minimum value among the integers written on the balls in the bag is $2$.
</p>

</section>

</div>

</span>

</span>

</div>
