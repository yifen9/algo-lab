
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
You are given two trees $T$and $U$, each with $N$vertices numbered from $1$to $N$. The $i$-th edge of $T$connects vertices $u_i$and $v_i$. The $i$-th edge of $U$connects vertices $b_i$and $c_i$.

You are also given a length-$N$integer sequence $A=(A_1,A_2,\dots,A_N)$.
</p>

<p>
For $k = 1, 2, \dots, N$, solve the following subproblem.
</p>

<blockquote>

<p>
Does there exist a tuple of integers $(x_1, x_2, x_3, x_4)$that satisfies the following conditions? If so, find the minimum value of $\sum_{i=1}^4 A_{x_i}$for a tuple satisfying the conditions.
</p>

<ul>

<li>
$x_1, x_2, x_3, x_4$are all distinct.
</li>

<li>
$x_1, x_2, x_3, x_4$are all different from $k$.
</li>

<li>
For all integers $(i,j)$satisfying $1 \leq i \lt j \leq 4$, the $x_i x_j$path in $T$contains vertex $k$, and the $x_i x_j$path in $U$also contains vertex $k$.
</li>

</ul>

</blockquote>

<p>
You are given $t$test cases; solve the problem for each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq t \leq 10^5$
</li>

<li>
$5 \leq N \leq 10^5$
</li>

<li>
$1 \leq A_i \leq 10^9$
</li>

<li>
$1 \leq u_i \lt v_i \leq N$
</li>

<li>
$1 \leq b_i \lt c_i \leq N$
</li>

<li>
$T$and $U$are trees.
</li>

<li>
The sum of $N$over all test cases is at most $10^5$.
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
The input is given from Standard Input in the following format. Here, $\mathrm{case}_i$means the $i$-th test case.
</p>

<div>

$t$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_t$
</div>

<p>
For each test case, the input is given in the following format:
</p>

<div>

$N$$A_1$$A_2$$\dots$$A_N$$u_1$$v_1$$u_2$$v_2$$\vdots$$u_{N-1}$$v_{N-1}$$b_1$$c_1$$b_2$$c_2$$\vdots$$b_{N-1}$$c_{N-1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $t$lines. The $i$-th line should contain the answer for the $i$-th test case.

For each test case, output the answers to the subproblems in the order $k=1,2,\dots,N$, separated by spaces on one line.

For each subproblem, output $-1$if there does not exist a tuple of integers $(x_1, x_2, x_3, x_4)$satisfying the conditions, or output the minimum value of $\sum_{i=1}^4 A_{x_i}$for such a tuple if it exists.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2
5
20 26 1 25 213
1 5
3 5
2 5
4 5
4 5
1 5
2 5
3 5
20
1 2 4 8 16 32 64 128 256 512 1024 2048 4096 8192 16384 32768 65536 131072 262144 524288
1 2
2 3
1 4
1 5
2 6
3 7
3 8
3 9
2 10
1 11
8 12
6 13
5 14
11 15
13 16
1 17
7 18
9 19
15 20
1 2
2 3
2 4
4 5
2 6
1 7
6 8
3 9
3 10
7 11
7 12
1 13
3 14
3 15
8 16
1 17
3 18
2 19
1 20

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

-1 -1 -1 -1 72
70664 616 131968 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1

</div>

<p>
For the first test case, when $k=1,2,3,4$, there does not exist $(x_1, x_2, x_3, x_4)$satisfying the conditions. When $k=5$, $(x_1,x_2,x_3,x_4) = (1,2,3,4)$satisfies the conditions.
</p>

</section>

</div>

</span>

</span>

</div>
