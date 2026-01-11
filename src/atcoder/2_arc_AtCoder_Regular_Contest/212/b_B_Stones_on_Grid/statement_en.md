
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a grid with $N$rows and $N$columns. The cell at the $i$-th row from the top and $j$-th column from the left is called cell $(i,j)$.
You perform the following in order of $i=1,2,\ldots,M$:
</p>

<ul>

<li>
Operation $i$: Choose either to place one stone on cell $(x_i, y_i)$or not. If you place a stone, a cost of $c_i$is incurred; otherwise, no cost is incurred.
</li>

</ul>

<p>
However, 
<strong>
you must place a stone in operation $1$
</strong>
.
</p>

<p>
Determine whether the following goal can be achieved, and if it can, find the minimum sum of costs incurred.
</p>

<ul>

<li>
Goal : For every $i \ (1 \leq i \leq N)$, the number of stones placed in the $i$-th row is equal to the number of stones placed in the $i$-th column.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N, M \le 2 \times 10^5$
</li>

<li>
$1 \le x_i, y_i \le N$
</li>

<li>
$1 \le c_i \le 10^9$
</li>

<li>
$(x_i, y_i)$are distinct.
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

$N$$M$$x_1$$y_1$$c_1$$x_2$$y_2$$c_2$$\vdots$$x_M$$y_M$$c_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If it is impossible to achieve the goal, output `-1`.
If it is possible, output the minimum sum of costs incurred.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 5
2 4 5
4 1 2
2 1 3
3 3 9
1 2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

11

</div>

<p>
The goal can be achieved by choosing to place a stone in operations $1,2,5$.
</p>

<p>
The sum of costs in this case is $5+2+4=11$. The total cost cannot be less than $11$to achieve the goal, so the answer is $11$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 3
1 1 1000000000
2 2 100000000
3 3 10000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1000000000

</div>

<p>
You must place a stone in operation $1$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

2 1
1 2 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

-1

</div>

</section>

</div>

</span>

</span>

</div>
