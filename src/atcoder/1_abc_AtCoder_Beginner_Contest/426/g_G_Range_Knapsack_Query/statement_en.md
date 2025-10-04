
<div>

<span>

<span>

<p>
Score : $575$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$items numbered from $1$to $N$.
The 
<strong>
weight
</strong>
of item $i$is $W_i$and the 
<strong>
value
</strong>
is $V_i$.
</p>

<p>
You are given $Q$queries, so process them in order.
The $j$-th query is as follows:
</p>

<ul>

<li>
Integers $L_j, R_j, C_j\ (1\leq L_j\leq R_j\leq N)$are given.
When choosing some (possibly zero) items from items $L_j,L_j+1,\dots,R_j$such that the total weight does not exceed $C_j$, find the maximum possible total value of the chosen items.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N \leq 2\times 10^4$
</li>

<li>
$1\leq Q \leq 2\times 10^5$
</li>

<li>
$1\leq W_i \leq 500$
</li>

<li>
$1\leq V_i \leq 10^9$
</li>

<li>
$1\leq L_j \leq R_j \leq N$
</li>

<li>
$1\leq C_j \leq 500$
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

$N$$W_1$$V_1$$W_2$$V_2$$\vdots$$W_N$$V_N$$Q$$L_1$$R_1$$C_1$$L_2$$R_2$$C_2$$\vdots$$L_Q$$R_Q$$C_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.
The $i$-th line $(1\leq i \leq Q)$should contain the answer for the $i$-th query.
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
3 4
5 8
1 2
2 3
3
1 4 7
2 4 10
1 2 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

11
13
0

</div>

<p>
For the first query, among items $1,2,3,4$, if you choose items $2,4$, the total weight is $5+2=7$, which does not exceed $C_1=7$, and the total value is $8+3=11$. This is the maximum.
</p>

<p>
For the second query, even if you choose all items $2,3,4$, the total weight is $5+1+2=8$, which does not exceed $C_2=10$, and you can achieve a total value of $8+2+3=13$.
</p>

<p>
For the third query, both items $1,2$have weights exceeding $C_3=2$, so you cannot choose any item, and the maximum total value is $0$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

8
167 430302156
22 623690081
197 476190629
176 24979445
22 877914575
247 211047202
232 822804784
25 628894325
8
6 8 176
3 5 80
1 7 310
4 8 368
4 5 218
3 4 431
4 6 228
1 1 239

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

628894325
877914575
2324409440
2329613684
902894020
501170074
902894020
430302156

</div>

</section>

</div>

</span>

</span>

</div>
