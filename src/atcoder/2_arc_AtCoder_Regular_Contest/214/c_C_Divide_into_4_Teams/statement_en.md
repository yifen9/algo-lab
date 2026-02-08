
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$people numbered $1, \dots ,N$. The 
<strong>
strength
</strong>
of person $i$is $P_i$.
</p>

<p>
Each person is assigned to one of the teams $A,B,C,D$to form four teams. There are $4^N$ways to form teams; among these, find the number, modulo $998244353$, of formations that satisfy all of the following conditions.
</p>

<ul>

<li>
Each of the teams $A,B,C,D$has at least one person.
</li>

<li>
The sum of the strengths of the people in team $A$equals the sum of the strengths of the people in team $B$.
</li>

<li>
The sum of the strengths of the people in team $C$equals the sum of the strengths of the people in team $D$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$4 \le N \le 500$
</li>

<li>
$1 \le P_i$
</li>

<li>
$\sum_{1 \le i \le N} P_i \le 10^5$
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

$N$$P_1$$P_2$$\ldots$$P_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the number, modulo $998244353$, of formations that satisfy the conditions in the problem statement.
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
1 1 2 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

8

</div>

<p>
The following eight team formations satisfy the conditions.
</p>

<table>

<thead>

<tr>

<th>

</th>

<th>
Person $1$
</th>

<th>
Person $2$
</th>

<th>
Person $3$
</th>

<th>
Person $4$
</th>

</tr>

</thead>

<tbody>

<tr>

<td>
Formation $1$
</td>

<td>
A
</td>

<td>
B
</td>

<td>
C
</td>

<td>
D
</td>

</tr>

<tr>

<td>
Formation $2$
</td>

<td>
B
</td>

<td>
A
</td>

<td>
C
</td>

<td>
D
</td>

</tr>

<tr>

<td>
Formation $3$
</td>

<td>
A
</td>

<td>
B
</td>

<td>
D
</td>

<td>
C
</td>

</tr>

<tr>

<td>
Formation $4$
</td>

<td>
B
</td>

<td>
A
</td>

<td>
D
</td>

<td>
C
</td>

</tr>

<tr>

<td>
Formation $5$
</td>

<td>
C
</td>

<td>
D
</td>

<td>
A
</td>

<td>
B
</td>

</tr>

<tr>

<td>
Formation $6$
</td>

<td>
C
</td>

<td>
D
</td>

<td>
B
</td>

<td>
A
</td>

</tr>

<tr>

<td>
Formation $7$
</td>

<td>
D
</td>

<td>
C
</td>

<td>
A
</td>

<td>
B
</td>

</tr>

<tr>

<td>
Formation $8$
</td>

<td>
D
</td>

<td>
C
</td>

<td>
B
</td>

<td>
A
</td>

</tr>

</tbody>

</table>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

9
1 2 3 4 5 6 7 8 9

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

<p>
No formations satisfy the conditions.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

24
1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

289359125

</div>

</section>

</div>

</span>

</span>

</div>
