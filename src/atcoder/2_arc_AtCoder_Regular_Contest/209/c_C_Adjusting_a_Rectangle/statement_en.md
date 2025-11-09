
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
You are given positive integers $N, X$and integer sequences of length $N$: $S = (S_1, S_2, \dots, S_N), P = (P_1, P_2, \dots, P_N)$.
Here, each element of $P$is $1$or $-1$.
</p>

<p>
You are given $Q$queries. In each query, you are given integers $l, r$satisfying $1 \leq l \leq r \leq N$, and you play the following game:
</p>

<ul>

<li>
Initially, your score is $0$, and integers $a, b$are initialized as $a = 1, b = 1$.
</li>

<li>
For $i = l, l+1, \dots, r$in this order, perform the following operation:
<ul>

<li>
If $i$is even, replace the value of $a$with any integer between $1$and $X$(inclusive); if $i$is odd, replace the value of $b$with any integer between $1$and $X$(inclusive).
</li>

<li>
After that, if $ab \geq S_i$, add $P_i$to your score. Otherwise, the score does not change. Note that $P_i$can be negative.
</li>

</ul>

</li>

</ul>

<p>
For each query, find the maximum possible value of your score when the game ends.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N, X, Q \le 10^5$
</li>

<li>
$1 \le S_i \le 10^5$
</li>

<li>
$P_i = 1$or $P_i = -1$.
</li>

<li>
For each query, $1 \le l \le r \le N$.
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

$N$$X$$Q$$S_1$$S_2$$\ldots$$S_N$$P_1$$P_2$$\ldots$$P_N$$\text{query}_1$$\text{query}_2$$\vdots$$\text{query}_Q$
</div>

<p>
Each query is given in the following format:
</p>

<div>

$l$$r$
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
The $i$-th line should contain the maximum possible value of your score when the game ends in the $i$-th query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

9 4 4
3 11 10 12 5 7 3 9 16
1 1 -1 1 -1 1 -1 1 1
5 9
1 4
5 5
2 8

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
3
0
1

</div>

<p>
In the first query, you can make the score $2$when the game ends by the following procedure:
</p>

<table>

<thead>

<tr>

<th>
$i$
</th>

<th>
Operation
</th>

<th>
$a$
</th>

<th>
$b$
</th>

<th>
Score
</th>

</tr>

</thead>

<tbody>

<tr>

<td>
-
</td>

<td>

</td>

<td>
$1$
</td>

<td>
$1$
</td>

<td>
$0$
</td>

</tr>

<tr>

<td>
$5$
</td>

<td>
Replace the value of $b$with $4$. Since $ab < S_5 \, (= 5)$, the score does not change.
</td>

<td>
$1$
</td>

<td>
$4$
</td>

<td>
$0$
</td>

</tr>

<tr>

<td>
$6$
</td>

<td>
Replace the value of $a$with $2$. Since $ab \geq S_6 \, (= 7)$, add $P_6 \, (= 1)$to the score.
</td>

<td>
$2$
</td>

<td>
$4$
</td>

<td>
$1$
</td>

</tr>

<tr>

<td>
$7$
</td>

<td>
Replace the value of $b$with $3$. Since $ab \geq S_7 \, (= 3)$, add $P_7 \, (= -1)$to the score.
</td>

<td>
$2$
</td>

<td>
$3$
</td>

<td>
$0$
</td>

</tr>

<tr>

<td>
$8$
</td>

<td>
Replace the value of $a$with $4$. Since $ab \geq S_8 \, (= 9)$, add $P_8 \, (= 1)$to the score.
</td>

<td>
$4$
</td>

<td>
$3$
</td>

<td>
$1$
</td>

</tr>

<tr>

<td>
$9$
</td>

<td>
Replace the value of $b$with $4$. Since $ab \geq S_9 \, (= 16)$, add $P_9 \, (= 1)$to the score.
</td>

<td>
$4$
</td>

<td>
$4$
</td>

<td>
$2$
</td>

</tr>

</tbody>

</table>

<p>
It is impossible to make the score $3$or more when the game ends, so output $2$.
</p>

</section>

</div>

</span>

</span>

</div>
