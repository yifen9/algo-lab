
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
You are given a tree $T$with $N$vertices numbered $1$to $N$. The $i$-th edge connects vertices $A_i$and $B_i$.
</p>

<p>
For a positive integer $k$, define a "centipede graph of length $k$" as a graph with $3k$vertices obtained by the following procedure:
</p>

<ul>

<li>
Prepare a path graph with $k$
<strong>
vertices
</strong>
.
</li>

<li>
For each vertex $v$of the path graph, add two new vertices adjacent only to $v$.
</li>

</ul>

<p>
For example, a centipede graph of length $4$is as shown in the figure below.
</p>

<p>

<img src="https://img.atcoder.jp/abc447/574f669df50f1e1b96042142eef82ae9.png">

</img>

</p>

<p>
Find the maximum $x$such that a "centipede graph of length $x$" is contained as a subgraph of tree $T$.
</p>

<p>
$Q$test cases are given; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le Q$
</li>

<li>
$3 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le A_i, B_i \le N$
</li>

<li>
The given graph is a tree.
</li>

<li>
The sum of $N$over all test cases is at most $2 \times 10^5$.
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

$Q$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_Q$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_{N-1}$$B_{N-1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.
</p>

<p>
The $i$-th line should contain the answer for the $i$-th test case.
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
8
1 3
2 4
2 5
2 6
3 5
4 7
5 8
5
1 5
1 2
1 3
3 4
15
13 3
4 13
11 1
14 9
9 13
13 6
1 10
7 9
13 2
10 5
3 12
15 13
9 10
12 8

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

</div>

<p>
For the first test case, the graph consisting of the six vertices $2,3,4,5,6,8$forms a "centipede graph of length $2$".
</p>

<p>
No centipede graph of length $3$or more is contained as a subgraph, so the answer is $2$. Thus, output $2$.
</p>

</section>

</div>

</span>

</span>

</div>
