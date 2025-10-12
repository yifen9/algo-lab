
<div>

<span>

<span>

<p>
Score : $425$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a directed graph with $N$vertices and $M$edges. The vertices are numbered from $1$to $N$, and the $i$-th edge is a directed edge from vertex $U_i$to vertex $V_i$. Here, the out-degree of each vertex is at least $1$.
</p>

<p>
Also, each vertex has a character written on it, and the character written on vertex $i$is $S_i$. Here, $S_i$refers to the $i$-th character of $S$. 
</p>

<p>
Alice and Bob play the following game on this graph using one piece:
</p>

<ul>

<li>

<p>
Initially, the piece is placed on vertex $1$, and they alternately perform the following operation $K$times each, with Alice going first and Bob going second.
</p>

<ul>

<li>
Let $u$be the vertex where the piece is currently placed. Choose a vertex $v$such that there is an edge from vertex $u$to vertex $v$, and move the piece to vertex $v$.
</li>

</ul>

</li>

<li>

<p>
Let $v$be the vertex where the piece is finally placed. If $S_v = $`A`, Alice wins; if $S_v = $`B`, Bob wins.
</p>

</li>

</ul>

<p>
Find the winner of the game when both players play optimally.
</p>

<p>
In each input, you are given $T$test cases. Solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T$
</li>

<li>
$2 \leq N, M \leq 2 \times 10^5$
</li>

<li>
$1 \leq K \leq 10$
</li>

<li>
$S$is a string of length $N$consisting of `A`and `B`.
</li>

<li>
$1 \leq U_i, V_i \leq N$
</li>

<li>
$(U_i, V_i) \neq (U_j, V_j)$if $i \neq j$.
</li>

<li>
The out-degree of each vertex is at least $1$.
</li>

<li>
The sum of $N$over all test cases in a single input is at most $2 \times 10^5$.
</li>

<li>
The sum of $M$over all test cases in a single input is at most $2 \times 10^5$.
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

$T$$\text{case}_1$$\text{case}_2$$\ldots$$\text{case}_T$
</div>

<p>
Here, $\text{case}_i$represents the $i$-th test case, and each test case is given in the following format:
</p>

<div>

$N$$M$$K$$S$$U_1$$V_1$$U_2$$V_2$$\vdots$$U_M$$V_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $T$lines. The $i$-th line should contain `Alice`if Alice wins when both players play optimally in the $i$-th test case, and `Bob`if Bob wins.
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
4 6 2
AABB
1 2
2 3
3 1
3 3
3 4
4 2
4 6 2
ABAB
1 2
2 3
3 1
3 3
3 4
4 2
5 8 3
ABABB
1 2
2 2
2 3
3 1
3 4
4 4
4 5
5 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Alice
Bob
Bob

</div>

<p>
We will explain an example of how the game proceeds in the first test case. Here, both players do not necessarily play optimally.
</p>

<ul>

<li>
Initially, the piece is placed on vertex $1$.
</li>

<li>
Alice moves the piece to vertex $2$.
</li>

<li>
Bob moves the piece to vertex $3$.
</li>

<li>
Alice moves the piece to vertex $3$.
</li>

<li>
Bob moves the piece to vertex $1$.
</li>

</ul>

<p>
At this point, $S_1 =$`A`, so Alice wins.
</p>

</section>

</div>

</span>

</span>

</div>
