
<div>

<span>

<span>

<p>
Score : $1100$points
</p>

<div>

<section>

### **Problem Statement**

<p>
A sequence that can be obtained as $A$by performing the following operations is called a 
<strong>
special sequence
</strong>
:
</p>

<ul>

<li>
Prepare an undirected graph consisting of $N$vertices and $0$edges, and a sequence $A$of length $0$.
</li>

<li>
Prepare queries for integers $i,j$satisfying $1 \leq i < j \leq N$and $q \in \{1,2\}$:
</li>

<ul>

<li>
When $q=1$, connect vertices $i$and $j$with an edge.
</li>

<li>
When $q=2$, append $1$to the end of $A$if vertices $i$and $j$are connected, and append $0$otherwise.
</li>

</ul>

<li>
There are $N(N-1)$possible queries; rearrange them in any order and process them in that order.
</li>

</ul>

<p>
You are given a sequence $B$of length $\frac{N(N-1)}{2}$consisting of $0$and $1$.
You can perform the following operation on $B$any number of times:
</p>

<ul>

<li>
Choose an integer $i$satisfying $1 \leq i \leq \frac{N(N-1)}{2}-1$, and swap $B_i$and $B_{i+1}$.
</li>

</ul>

<p>
Determine whether it is possible to make $B$a special sequence, and if possible, find the minimum number of operations required.
</p>

<p>
Solve $T$test cases per input.
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
$2 \leq N \leq 500$
</li>

<li>
$|B| =\frac{N(N-1)}{2}$
</li>

<li>
$0 \leq B_i \leq 1$
</li>

<li>
The sum of $|B|$over all test cases is at most $3 \times 10^5$.
</li>

<li>
The sum of $N^3$over all test cases is at most $500^3$.
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

$T$$case_1$$case_2$$\vdots$$case_T$
</div>

<p>
Each case is given in the following format:
</p>

<div>

$N$$B_1$$B_2$$\ldots$$B_{\frac{N(N-1)}{2}}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines in total.
The $t$-th line should contain the minimum number of operations required to make $B$a special sequence for the $t$-th test case if it is possible to do so, and `-1`otherwise.
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
4
1 1 0 1 1 0
2
1
3
0 0 0
5
1 1 1 1 1 1 1 1 1 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
0
0
3

</div>

<p>
In the first test case, if the queries are processed in the order $(q,i,j)=(1,1,4),$$(2,1,4),$$(1,2,4),$$(2,1,2),$$(1,1,2),$$(2,2,3),$$(2,2,4),$$(2,3,4),$$(1,3,4),$$(1,1,3),$$(2,1,3),$$(1,2,3)$, the resulting sequence is $(1,1,0,1,0,1)$, and $B$can be changed to this sequence by performing the operation once. Also, $(1,1,0,1,1,0)$is not a special sequence, so the answer is $1$.
</p>

</section>

</div>

</span>

</span>

</div>
