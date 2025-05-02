
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
There are $N$towns, numbered $1,2,\ldots,N$, arranged in a line in this order.
</p>

<p>
There are $N-1$roads connecting adjacent towns: road $j\,(1 \leq j \leq N-1)$connects towns $j$and $j+1$. For each road $j$, you can set a 
<strong>
strength
</strong>
$w_j$(an integer that may be negative).
</p>

<p>
When a person travels along a road, their 
<strong>
stamina
</strong>
changes. Specifically, if a person with stamina $x$travels along road $j$, their stamina becomes $x + w_j$.
</p>

<p>
There are $M$people who will now move between these towns.
</p>

<p>
Person $i\,(1 \le i \le M)$starts with stamina $0$at town $S_i$and travels to town $T_i$via the shortest path.
It is guaranteed that $|S_i - T_i| > 1$. Also, $(S_i, T_i) \neq (S_j, T_j)$if $i \neq j$.
</p>

<p>
Person $i$’s requirement is as follows:
</p>

<blockquote>

<p>
When departing Town $S_i$and when arriving at Town $T_i$, their stamina should be exactly $0$. At every other town, their stamina should always be a positive integer.
</p>

</blockquote>

<p>
Assume that there are no changes to stamina other than those due to traveling along roads as described above.
</p>

<p>
Process $Q$queries. For the $k$-th query $(1 \le k \le Q)$, if it is possible to set the strengths of the roads so that the requirements of all people $L_k, L_k + 1, \ldots, R_k$are satisfied, print `Yes`; otherwise, print `No`.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3 \le N \le 4 \times 10^5$
</li>

<li>
$1 \le M \le 2 \times 10^5$
</li>

<li>
$1 \le Q \le 2 \times 10^5$
</li>

<li>
$1 \le S_i, T_i \le N$
</li>

<li>
$|S_i - T_i| > 1$
</li>

<li>
$(S_i, T_i) \neq (S_j, T_j)\,(i \neq j)$
</li>

<li>
$1 \le L_k \le R_k \le M$
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

$N$$M$$Q$$S_1$$T_1$$S_2$$T_2$$\vdots$$S_M$$T_M$$L_1$$R_1$$L_2$$R_2$$\vdots$$L_Q$$R_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $Q$lines.
</p>

<p>
The $k$-th line should contain `Yes`if there is a way to set the strengths of the roads so that the requirements of all people $L_k, L_k + 1, \ldots, R_k$are satisfied, and `No`otherwise.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 4 2
4 2
1 3
3 5
2 4
1 3
2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
No

</div>

<p>
For the first query, consider setting the strengths of roads $1, 2, 3, 4$to $1, -1, 1, -1$, respectively.
</p>

<ul>

<li>
Person $1$starts at town $4$with stamina $0$, visits town $3$with stamina $1$, and arrives at town $2$with stamina $0$.
</li>

<li>
Person $2$starts at town $1$with stamina $0$, visits town $2$with stamina $1$, and arrives at town $3$with stamina $0$.
</li>

<li>
Person $3$starts at town $3$with stamina $0$, visits town $4$with stamina $1$, and arrives at town $5$with stamina $0$.
</li>

</ul>

<p>
Thus, this configuration satisfies the requirements of persons $1,2,3$, so print `Yes`on the first line.
</p>

<p>
For the second query, it is impossible to satisfy the requirements of persons $2,3,4$simultaneously, so print `No`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

7 6 3
1 5
2 4
4 6
7 1
5 3
1 6
1 6
4 4
2 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No
Yes
Yes

</div>

</section>

</div>

</span>

</span>

</div>
