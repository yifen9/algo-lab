
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
There are $N$children, numbered $1$to $N$.
</p>

<p>
Child $i$has $A_i$candies.
</p>

<p>
Your goal is to execute the following operation as few times as possible so that eventually all $N$children have the same number of candies.
</p>

<ul>

<li>
Choose two distinct children $x,y$, and choose a positive integer $z$not exceeding the number of candies child $x$has. Take $z$candies from child $x$and give them to child $y$.
</li>

</ul>

<p>
Determine whether there exists a sequence of operations such that eventually all $N$children have the same number of candies. If it exists, find one such sequence with the minimum number of operations.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 20$
</li>

<li>
$1 \leq A_i \leq 10^8$
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

$N$$A_1$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If there is no sequence of operations such that eventually all $N$children have the same number of candies, output `-1`.
</p>

<p>
If it exists, output one with the minimum number of operations in the following format:
</p>

<div>

$q$$x_1$$y_1$$z_1$$\vdots$$x_q$$y_q$$z_q$
</div>

<p>
Here, $q$represents the number of operations, and $x_i,y_i,z_i$represent the values of $x,y,z$chosen in the $i$-th operation.
</p>

<p>
If there are multiple solutions, outputting any of them will be considered correct.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4
1 7 4 8

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
2 3 1
2 4 1
4 1 4

</div>

<p>
In this sample output, the operations are executed as follows:
</p>

<ol>

<li>
Take $1$candy from child $2$and give it to child $3$. Immediately after this, the number of candies each child has is $1,6,5,8$.
</li>

<li>
Take $1$candy from child $2$and give it to child $4$. Immediately after this, the number of candies each child has is $1,5,5,9$.
</li>

<li>
Take $4$candies from child $4$and give them to child $1$. Immediately after this, the number of candies each child has is $5,5,5,5$.
</li>

</ol>

<p>
Eventually, all $N$children have exactly five candies each.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2
100 3

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

</span>

</span>

</div>
