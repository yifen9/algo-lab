
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
There are $N$permutations of $(1,2,\dots,L)$. The $i$-th permutation is $P_i$, and the $j$-th element of $P_i$is $P_{i,j}$($1 \le j \le L$).
</p>

<p>
Initially, you have $A = (1,2,\dots,L)$, and your initial amount of money is $0$yen. From now on, for $i = 1,2,\dots,N$in this order, you will perform the following operation:
</p>

<ol>

<li>
First, perform zero or one swap of two adjacent elements in $A$.
<ul>

<li>
Specifically, “a swap of two adjacent elements in $A$” means choosing $j$with $1 \le j \le L-1$, and swapping $A_j$and $A_{j+1}$.
</li>

</ul>

</li>

<li>
Then, if $A$is equal to $P_i$, you gain $C_i$yen.
</li>

</ol>

<p>
Find the maximum possible amount of money you can have at the end.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 3 \times 10^4$
</li>

<li>
$1 \leq L \leq 9$
</li>

<li>
$0 \leq C_i \leq 10^4$
</li>

<li>
Each $P_i$is a permutation of $(1,2,\dots,L)$.
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

$N$$L$$C_1$$P_{1,1}$$P_{1,2}$$\dots$$P_{1,L}$$C_2$$P_{2,1}$$P_{2,2}$$\dots$$P_{2,L}$$\vdots$$C_N$$P_{N,1}$$P_{N,2}$$\dots$$P_{N,L}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 3
200 2 1 3
400 3 1 2
300 2 3 1
100 3 2 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

600

</div>

<p>
By doing the operations as follows, you can end up with $600$yen.
</p>

<ul>

<li>
For $i=1$: swap $A_1$and $A_2$, so $A=(2,1,3)$. We have $A=P_1$, so you gain $200$yen.
</li>

<li>
For $i=2$: swap $A_2$and $A_3$, so $A=(2,3,1)$. We have $A \neq P_2$.
</li>

<li>
For $i=3$: do not swap, so $A=(2,3,1)$. We have $A=P_3$, so you gain $300$yen.
</li>

<li>
For $i=4$: swap $A_1$and $A_2$, so $A=(3,2,1)$. We have $A=P_4$, so you gain $100$yen.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2 1
0 1
10000 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

10000

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

1 9
2025 2 4 6 8 7 5 1 9 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

10 5
2615 5 1 3 4 2
4275 1 3 2 5 4
4331 3 1 5 2 4
1457 3 5 1 2 4
2222 1 3 2 4 5
5051 2 4 5 3 1
1082 2 3 1 5 4
1579 4 1 5 2 3
2855 5 1 3 2 4
5848 2 4 3 1 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

12345

</div>

</section>

</div>

</span>

</span>

</div>
