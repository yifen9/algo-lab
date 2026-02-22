
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
You are given a tree with $N$vertices numbered $1$to $N$. The $i$-th edge ($1 \le i \le N - 1$) connects vertices $A_i$and $B_i$.
For a path in this tree, define the score of the path as the distance from the path to the farthest vertex.
Here, the distance from a path is defined as the minimum distance to a vertex on the path.
</p>

<p>
A path with the minimum score is called a good path.
</p>

<p>
For each $k = 1, 2, \ldots, N$, find the number of good paths with exactly $k$vertices.
Paths are distinguished only if their vertex sets differ.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le A_i < B_i \le N$($1 \le i \le N - 1$)
</li>

<li>
The given graph is a tree.
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

$N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_{N - 1}$$B_{N - 1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines.
</p>

<p>
The $k$-th line should contain the number of good paths with exactly $k$vertices.
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
1 2
2 3
2 4
3 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

0
1
3
2
0

</div>

<p>
The minimum score is $1$.
</p>

<p>
The good paths are the following six paths.
</p>

<ul>

<li>
The path with two vertices connecting vertices $2$and $3$
</li>

<li>
The path with three vertices connecting vertices $1$and $3$
</li>

<li>
The path with three vertices connecting vertices $2$and $5$
</li>

<li>
The path with three vertices connecting vertices $3$and $4$
</li>

<li>
The path with four vertices connecting vertices $1$and $5$
</li>

<li>
The path with four vertices connecting vertices $4$and $5$
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

8
1 2
2 3
2 4
3 5
5 6
3 7
7 8

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1
3
7
8
5
0
0
0

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5
1 2
2 3
3 4
4 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

0
0
0
0
1

</div>

</section>

</div>

</span>

</span>

</div>
