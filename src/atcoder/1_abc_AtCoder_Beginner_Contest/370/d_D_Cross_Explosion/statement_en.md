
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a grid with $H$rows and $W$columns. Let $(i, j)$denote the cell at the $i$-th row from the top and $j$-th column from the left.

Initially, there is one wall in each cell.

After processing $Q$queries explained below in the order they are given, find the number of remaining walls.
</p>

<p>
In the $q$-th query, you are given two integers $R_q$and $C_q$.

You place a bomb at $(R_q, C_q)$to destroy walls. As a result, the following process occurs.
</p>

<ul>

<li>
If there is a wall at $(R_q, C_q)$, destroy that wall and end the process.
</li>

<li>
If there is no wall at $(R_q, C_q)$, destroy the first walls that appear when looking up, down, left, and right from $(R_q, C_q)$. More precisely, the following four processes occur simultaneously:
<ul>

<li>
If there exists an $i \lt R_q$such that a wall exists at $(i, C_q)$and no wall exists at $(k, C_q)$for all $i \lt k \lt R_q$, destroy the wall at $(i, C_q)$.
</li>

<li>
If there exists an $i \gt R_q$such that a wall exists at $(i, C_q)$and no wall exists at $(k, C_q)$for all $R_q \lt k \lt i$, destroy the wall at $(i, C_q)$.
</li>

<li>
If there exists a $j \lt C_q$such that a wall exists at $(R_q, j)$and no wall exists at $(R_q, k)$for all $j \lt k \lt C_q$, destroy the wall at $(R_q, j)$.
</li>

<li>
If there exists a $j \gt C_q$such that a wall exists at $(R_q, j)$and no wall exists at $(R_q, k)$for all $C_q \lt k \lt j$, destroy the wall at $(R_q, j)$.
</li>

</ul>

</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq H, W$
</li>

<li>
$H \times W \leq 4 \times 10^5$
</li>

<li>
$1 \leq Q \leq 2 \times 10^5$
</li>

<li>
$1 \leq R_q \leq H$
</li>

<li>
$1 \leq C_q \leq W$
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

$H$$W$$Q$$R_1$$C_1$$R_2$$C_2$$\vdots$$R_Q$$C_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the number of remaining walls after processing all queries.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2 4 3
1 2
1 2
1 3

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
The process of handling the queries can be explained as follows:
</p>

<ul>

<li>
In the 1st query, $(R_1, C_1) = (1, 2)$. There is a wall at $(1, 2)$, so the wall at $(1, 2)$is destroyed.
</li>

<li>
In the 2nd query, $(R_2, C_2) = (1, 2)$. There is no wall at $(1, 2)$, so the walls at $(2,2),(1,1),(1,3)$, which are the first walls that appear when looking up, down, left, and right from $(1, 2)$, are destroyed.
</li>

<li>
In the 3rd query, $(R_3, C_3) = (1, 3)$. There is no wall at $(1, 3)$, so the walls at $(2,3),(1,4)$, which are the first walls that appear when looking up, down, left, and right from $(1, 3)$, are destroyed.
</li>

</ul>

<p>
After processing all queries, there are two remaining walls, at $(2, 1)$and $(2, 4)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 5 5
3 3
3 3
3 2
2 2
1 2

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

4 3 10
2 2
4 1
1 1
4 2
2 1
3 1
1 3
1 2
4 3
4 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

2

</div>

</section>

</div>

</span>

</span>

</div>
