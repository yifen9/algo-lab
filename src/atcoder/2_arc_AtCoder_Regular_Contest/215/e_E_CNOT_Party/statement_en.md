
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
You are given binary strings $A = A_1 A_2 \ldots A_N$and $B = B_1 B_2 \ldots B_N$of length $N$.
</p>

<p>
You can perform $M$types of operations. The $i$-th type of operation is represented by a pair of integers $(x_i, y_i)$with $1 \le x_i, y_i \le N$, and it flips the value of $A_{y_i}$when $A_{x_i} = 1$. It is possible that $x_i = y_i$. Here, flipping means changing $0$to $1$or $1$to $0$.
</p>

<p>
Determine whether it is possible to convert $A$into a string equal to $B$by performing at most $2N$operations on $A$, and if so, construct one such way.
</p>

<p>
You are given $T$test cases; solve each one.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 2 \times 10^5$
</li>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le M \le 2 \times 10^5$
</li>

<li>
$A$and $B$are binary strings of length $N$.
</li>

<li>
$A \neq B$
</li>

<li>
$1 \le x_i \le N$($1 \le i \le M$)
</li>

<li>
$1 \le y_i \le N$($1 \le i \le M$)
</li>

<li>
The sum of $N$and $M$over all test cases is at most $2 \times 10^5$.
</li>

<li>
$T$, $N$, $M$, $x_i$, $y_i$are integers.
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$A$$B$$M$$x_1$$y_1$$x_2$$y_2$$\vdots$$x_M$$y_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output for the $T$test cases in order.
</p>

<p>
For each test case, output as follows.
</p>

<p>
If no sequence of operations satisfying the condition exists, output `-1`on a single line.
</p>

<p>
If a sequence of operations satisfying the condition exists, let $K$be the length of the sequence of operations and $C_i$be the index of the $i$-th operation performed, and output as follows:
</p>

<div>

$K$$C_1$$C_2$$\ldots$$C_K$
</div>

<p>
Here, $K$must be at most $2N$, and operation $i$must not be performed when $A_{x_i} = 0$.
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
4
0100
1010
4
1 2
2 1
2 3
4 3
2
10
01
1
1 2
2
01
00
3
1 1
1 2
2 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
2 3 1
-1
3
3 2 1

</div>

<p>
For the first test case, you can perform the operations as follows.
</p>

<ul>

<li>
Initially, $A = 0100$.
</li>

<li>
Perform operation $2$. Now, $A = 1100$.
</li>

<li>
Perform operation $3$. Now, $A = 1110$.
</li>

<li>
Perform operation $1$. Now, $A = 1010$.
</li>

</ul>

<p>
For the second test case, no matter what operations are performed, it is impossible to make $A_1$equal to $0$.
</p>

<p>
Note that, as in the third test case, $x_i = y_i$is possible.
</p>

</section>

</div>

</span>

</span>

</div>
