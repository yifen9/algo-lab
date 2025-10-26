
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
You are given a simple directed acyclic graph $G$with $N$vertices numbered $1$to $N$.
$G$has $M$edges, and the $i$-th edge is directed from vertex $x_i$to vertex $y_i$.
</p>

<p>
A permutation $P=(P_1,P_2,\ldots,P_N)$of $(1,2,\ldots,N)$that satisfies the following condition is called a 
<strong>
special permutation
</strong>
:
</p>

<ul>

<li>
$P_{x_i} \lt P_{y_i}$for all $i=1,2,\cdots,M$.
</li>

</ul>

<p>
You are given a special permutation $P$.
Takahashi and Aoki will play a game using it.
Takahashi knows the value of each term of $P$, but Aoki only knows that $P$is a special permutation.
Both of them know $G$.
Takahashi selects some terms of $P$and tells Aoki their positions and values.
Find the minimum number of terms that Takahashi needs to tell Aoki so that Aoki can determine the values of all terms of $P$.
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
$1 \leq T \leq 10^4$
</li>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$0 \leq M \leq 2 \times 10^5$
</li>

<li>
$1 \leq x_i,y_i \leq N$
</li>

<li>
The given graph $G$is a simple directed acyclic graph.
</li>

<li>
$1 \leq P_i \leq N$
</li>

<li>
$P_1,P_2,\ldots,P_N$are pairwise distinct.
</li>

<li>
$P_{x_i} \lt P_{y_i}$
</li>

<li>
The sum of $N$over all test cases is at most $2 \times 10^5$.
</li>

<li>
The sum of $M$over all test cases is at most $2 \times 10^5$.
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

$N$$M$$x_1$$y_1$$x_2$$y_2$$\vdots$$x_M$$y_M$$P_1$$P_2$$\ldots$$P_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines in total.
The $t$-th line should contain the answer for the $t$-th test case.
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
5 4
3 4
4 1
3 1
5 2
5 4 1 2 3
4 0
4 2 1 3
10 15
6 2
8 5
4 9
7 10
3 7
5 6
8 9
3 5
5 2
8 2
3 9
5 9
10 2
3 2
7 4
8 9 2 6 4 5 3 1 10 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
3
6

</div>

<p>
In the first case, if Takahashi tells that $P_1=5, \; P_4=2$, Aoki can determine all terms of $P$. Also, if Takahashi tells only one term of $P$, Aoki cannot determine all terms of $P$.
</p>

</section>

</div>

</span>

</span>

</div>
