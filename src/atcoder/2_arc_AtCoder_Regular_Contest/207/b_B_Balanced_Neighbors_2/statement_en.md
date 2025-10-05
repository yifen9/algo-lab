
<div>

<span>

<span>

<p>
Score : $800$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer $N$.
Determine whether there exists a simple connected undirected graph with $N$vertices numbered $1$to $N$that satisfies the following condition, and if it exists, show one such graph.
</p>

<ul>

<li>
There exists an integer $X$such that for any vertex $v$, the sum of the numbers of all vertices other than $v$that can be reached from $v$by traversing an edge once or twice is $X$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \le N \le 200$
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

$N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If there does not exist a simple connected undirected graph with $N$vertices satisfying the condition in the problem statement, print `-1`.
If it exists, print the number of edges $M$on the first line. On the $i$-th of the following $M$lines, print two integers. These represent the vertex numbers of the endpoints of the $i$-th edge.
</p>

<p>
Any constructed graph that satisfies the condition will be accepted.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

12

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

24
1 2
2 3
3 1
1 4
4 5
5 1
2 6
6 8
8 2
3 7
7 9
9 3
4 6
6 10
10 4
5 7
7 11
11 5
8 9
9 12
12 8
10 11
11 12
12 10

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1

</div>

<p>
If there does not exist a graph satisfying the condition, print `-1`.
</p>

</section>

</div>

</span>

</span>

</div>
