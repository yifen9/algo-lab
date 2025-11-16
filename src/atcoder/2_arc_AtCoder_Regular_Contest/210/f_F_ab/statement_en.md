
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
You are given an integer sequence $A=(A_1,A_2,\ldots,A_N)$. Also, you are given positive integers $a,b,s,t$. It is guaranteed that $a$and $b$are 
<strong>
coprime
</strong>
.
</p>

<p>
You can perform the following four types of operations on $A$:
</p>

<ul>

<li>
Choose an integer $i$satisfying $1\leq i\leq N$and add $a$to $A_i$. This operation costs $s$.
</li>

<li>
Choose an integer $i$satisfying $1\leq i\leq N$and subtract $a$from $A_i$. This operation costs $s$.
</li>

<li>
Choose an integer $i$satisfying $1\leq i\leq N$and add $b$to $A_i$. This operation costs $t$.
</li>

<li>
Choose an integer $i$satisfying $1\leq i\leq N$and subtract $b$from $A_i$. This operation costs $t$.
</li>

</ul>

<p>
Answer $Q$queries. In the $q$-th query, you are given an integer $B_q$, so find the following value modulo $998244353$:
</p>

<ul>

<li>
The minimum total cost required to make $A_{1}=A_{2}=\cdots=A_{N}=B_q$hold. It can be proved that it is possible to make $A_{1}=A_{2}=\cdots=A_{N}=B_q$hold.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N\leq 2\times 10^5$
</li>

<li>
$1\leq Q\leq 2\times 10^5$
</li>

<li>
$1\leq a,b,s,t\leq 5\times 10^8$
</li>

<li>
$a$and $b$are coprime.
</li>

<li>
$1\leq A_i\leq 5\times 10^8$
</li>

<li>
$1\leq B_q\leq 5\times 10^8$
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

$N$$Q$$a$$b$$s$$t$$A_1$$A_2$$\ldots$$A_N$$B_1$$B_2$$\ldots$$B_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$values separated by spaces.
</p>

<p>
The $q$-th value should be the minimum total cost, modulo $998244353$, required to make $A_{1}=A_{2}=\cdots=A_{N}=B_q$hold.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

1 5
3 5 4 3
3
1 2 3 4 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

7 11 0 11 7

</div>

<ul>

<li>
By performing operations $+a$, $-b$on $A_1$in order, we can make $A=(1)$. The total cost is $4+3=7$.
</li>

<li>
By performing operations $-a$, $-a$, $+b$on $A_1$in order, we can make $A=(2)$. The total cost is $4+4+3=11$.
</li>

<li>
$A=(3)$from the beginning. The total cost is $0$.
</li>

<li>
By performing operations $+a$, $+a$, $-b$on $A_1$in order, we can make $A=(4)$. The total cost is $4+4+3=11$.
</li>

<li>
By performing operations $-a$, $+b$on $A_1$in order, we can make $A=(5)$. The total cost is $4+3=7$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 1
3 5 4 3
1 2 3
4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

22

</div>

<ul>

<li>
By performing operations $+a$on $A_1$, $+b$, $-a$on $A_2$, and $+a,+a,-b$on $A_3$in order, we can make $A=(4,4,4)$. The total cost is $22$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5 5
1234 4321 5 5
1 10 100 1000 10000
123 4567 89012345 6 789

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

45340 42530 531725 35135 41690

</div>

</section>

</div>

</span>

</span>

</div>
