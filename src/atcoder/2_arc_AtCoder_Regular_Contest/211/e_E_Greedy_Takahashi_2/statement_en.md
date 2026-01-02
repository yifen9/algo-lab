
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
You are given a positive integer $N$and a permutation $P$of $(1,2,\dots,N)$.
</p>

<p>
When there is a tree with $N$vertices numbered $1,2,\dots,N$, Snuke and Takahashi move according to the following rules:
</p>

<ul>

<li>
Snuke specifies a permutation $Q$of $(1,2,\dots,N)$such that the sequence returned by Takahashi, when following the rules below, is lexicographically maximum.
</li>

<li>
Takahashi, who is at vertex $1$of the tree, first receives $Q$from Snuke and initializes an integer sequence $R$with the length-$1$sequence $(Q_1)$. Then, he moves $N-1$times as follows, and returns the final $R$:
<ul>

<li>
Visit the vertex $i$with the smallest $Q_i$among vertices that are adjacent to a previously visited vertex but have not yet been visited (it can be proved that there is always exactly one such vertex). Then, append $Q_i$to the end of $R$.
</li>

</ul>

</li>

</ul>

<p>
Here, vertex $1$is considered to have been visited initially.
</p>

<p>
Determine whether there exists a tree such that Takahashi returns $P$.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 10^5$
</li>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$P$is a permutation of $(1,2,\dots,N)$.
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$P_1$$P_2$$\ldots$$P_N$
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
The $i$-th line should contain `Yes`if there exists a tree satisfying the conditions for the $i$-th test case, and `No`otherwise.
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
4 2 3 1
4
4 1 3 2
11
11 8 9 6 7 10 3 4 5 1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
No
Yes

</div>

<p>
For the first test case, a tree with four vertices having edges between vertices $1$-$2$, $1$-$3$, and $2$-$4$satisfies the conditions.
</p>

<p>
If Snuke specifies $Q=(4,3,2,1)$, Takahashi visits vertices $1,3,2,4$in this order and returns $R=(4,2,3,1)$. No matter what $Q$Snuke specifies, it is impossible to make Takahashi return a sequence lexicographically larger than $(4,2,3,1)$, so the sequence that ends up being returned is $(4,2,3,1)$.
</p>

<p>
For the second test case, it can be proved that there is no tree satisfying the conditions.
</p>

</section>

</div>

</span>

</span>

</div>
