
<div>

<span>

<span>

<p>
Score : $900$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given positive integers $N$and $K$.
</p>

<p>
There is a complete bipartite graph $G$with $N$vertices $l_1, l_2, \ldots, l_N$on the left and $N$vertices $r_1, r_2, \ldots, r_N$on the right. It has $N^2$edges; for each $(i, j)\ (1\leq i\leq N, 1\leq j\leq N)$, there is one undirected edge between vertices $l_i$and $r_j$.
</p>

<p>
Determine whether there exists a way to write an integer between $1$and $N^2$, inclusive, on each edge of $G$(where the $N^2$integers written are all distinct) such that the answer to the following problem is $K$, and if such a way exists, find one.
</p>

<blockquote>

<p>
Among all walks on graph $G$, we call a walk 
<strong>
good
</strong>
if the sequence of numbers written on the edges traversed, in the order they are traversed, is strictly increasing.
</p>

<p>
Find the maximum number of edges contained in a good walk.
</p>

</blockquote>

<p>
$T$test cases are given; solve each of them.
</p>

<details>

<summary>
What is a walk?
</summary>
A walk on graph $G$is a sequence of $k$vertices and $k-1$edges alternately arranged, $(v_1 ​ ,e_1 ​ ,v_2 ​ ,\ldots,v_{k−1} ​ ,e_{k−1} ​ ,v_k)$(where $k$is a positive integer), such that edge $e_i$connects vertices $v_i$and $v_{i+1}$.

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq T\leq 3000$
</li>

<li>
$1\leq N\leq 700$
</li>

<li>
$1\leq K\leq N^2$
</li>

<li>
The sum of $N^2$in each input is at most $5\times 10^5$.
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$K$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for $\mathrm{case}_1,\mathrm{case}_2,\ldots,\mathrm{case}_T$in this order in the following format.
</p>

<p>
If no valid way of writing exists, output `No`.
</p>

<p>
If a valid way exists, letting $A_{i,j}$be the integer written on the edge connecting vertices $l_i$and $r_j$,
</p>

<div>

Yes
$A_{1,1}$$A_{1,2}$$\ldots$$A_{1,N}$$A_{2,1}$$A_{2,2}$$\ldots$$A_{2,N}$$\vdots$$A_{N,1}$$A_{N,2}$$\ldots$$A_{N,N}$
</div>

<p>
output as above. $(A_{1,1},\ldots,A_{1,N},A_{2,1},\ldots,A_{2,N},\ldots,A_{N,1},\ldots,A_{N,N})$must be a permutation of $(1,2,\ldots,N^2)$.
</p>

<p>
If multiple solutions exist, any of them will be accepted.
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
2 1
2 3
3 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

No
Yes
1 2
3 4
Yes
2 9 7
4 5 6
1 8 3

</div>

<p>
For the first test case, no valid way of writing exists.
</p>

<p>
For the second test case, a good walk containing three edges is $r_1 \xrightarrow{1} l_1 \xrightarrow{2}r_2\xrightarrow{4}l_2$. No good walk contains four or more edges, so this output satisfies the condition.
</p>

<p>
For the third test case, a good walk containing five edges is $l_1 \xrightarrow{2} r_1 \xrightarrow{4}l_2\xrightarrow{6}r_3 \xrightarrow{7} l_1 \xrightarrow{9} r_2$. No good walk contains six or more edges, so this output satisfies the condition.
</p>

<p>

<img src="https://img.atcoder.jp/agc077/483f3ac7fef3640067cde0b569f0be80.png">

</img>

</p>

</section>

</div>

</span>

</span>

</div>
