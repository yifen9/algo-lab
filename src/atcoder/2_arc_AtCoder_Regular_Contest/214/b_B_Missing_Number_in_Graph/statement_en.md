
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
There is a connected simple undirected graph with $N$vertices and $M$edges, where the vertices are numbered $1, \dots ,N$and the edges are numbered $1, \dots ,M$.
Edge $i$connects vertices $A_i$and $B_i$.
Also, there are a total of $N+1$cards, one each with the integers from $0$to $N$written on them.
</p>

<p>
Snuke performed the following operations in order:
</p>

<ol>

<li>
Place one card on each vertex, and eat the remaining one card.
</li>

<li>
For each $i\ (1 \le i \le M)$, write on edge $i$the bitwise $\mathrm{XOR}$of the integers written on the two cards placed on vertices $A_i$and $B_i$. Let this integer be $X_i$.
</li>

<li>
Discard all cards placed on the vertices.
</li>

</ol>

<p>
Given the information about the graph ($N,M,A_1,\dots ,A_M,B_1,\dots ,B_M,X_1,\dots ,X_M$), determine the integer written on the card that Snuke ate. If it cannot be uniquely determined, output `-1`.
It is guaranteed that the given $X$can be obtained by the above operations.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

<details>

<summary>
What is bitwise $\mathrm{XOR}$?
    
</summary>

<p>
The bitwise $\mathrm{XOR}$of non-negative integers $A$and $B$, $A \oplus B$, is defined as follows:
        
</p>

<ul>

<li>
In the binary representation of $A \oplus B$, the digit in the $2^k$($k \geq 0$) place is $1$if exactly one of the digits in the $2^k$place in the binary representations of $A$and $B$is $1$, and $0$otherwise.
</li>

</ul>
For example, $3 \oplus 5 = 6$(in binary: $011 \oplus 101 = 110$).

In general, the bitwise $\mathrm{XOR}$of $k$non-negative integers $p_1, p_2, p_3, \dots, p_k$is defined as $(\dots ((p_1 \oplus p_2) \oplus p_3) \oplus \dots \oplus p_k)$, and it can be proved that this does not depend on the order of $p_1, p_2, p_3, \dots, p_k$.  
    
<p>

</p>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 10^4$
</li>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$0 \le M \le 2 \times 10^5$
</li>

<li>
$1 \le A_i,B_i \le N$
</li>

<li>
The given graph is a connected simple undirected graph.
</li>

<li>
$X_1,\dots ,X_M$can be obtained by the operations in the problem statement.
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$M$$A_1$$B_1$$X_1$$A_2$$B_2$$X_2$$\vdots$$A_M$$B_M$$X_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines.
</p>

<p>
The $i$-th line should contain the integer written on the card Snuke ate for the $i$-th test case if it can be uniquely determined, and `-1`otherwise.
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
1 2 3
1 0
4 4
2 1 4
1 3 5
1 4 7
2 3 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

0
-1
2

</div>

<p>
For the first test case, the graph is as shown below.
</p>

<p>

<img src="https://img.atcoder.jp/arc214/3ff6e65b4be3e9a4e483771d6fe27e35.png">

</img>

</p>

<p>
The possible pairs of integers written on the cards placed on vertices $1$and $2$are $(1,2)$and $(2,1)$; in either case, the integer written on the card Snuke ate is $0$.
</p>

<p>
For the second test case, there are two possible integers written on the card Snuke ate: $0$and $1$.
</p>

<p>
For the third test case, the graph is as shown below.
</p>

<p>

<img src="https://img.atcoder.jp/arc214/46b2a2846e7ed1a27553c71b7d760ef8.png">

</img>

</p>

</section>

</div>

</span>

</span>

</div>
