
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
You are given a positive integer $N$and a sequence $A = (A_0, A_1, \ldots, A_{2^N-1})$of $2^N$terms, where each $A_i$is an integer between $0$and $2^N-1$(inclusive) and $A_i\neq A_j$holds if $i\neq j$.
</p>

<p>
You can perform the following two kinds of operations on $A$:
</p>

<ul>

<li>
Operation $+$: For every $i$, change $A_i$to $(A_i + 1) \bmod 2^N$.
</li>

<li>
Operation $\oplus$: Choose an integer $x$between $0$and $2^N-1$. For every $i$, change $A_i$to $A_i\oplus x$.
</li>

</ul>

<p>
Here, $\oplus$denotes bitwise $\mathrm{XOR}$.
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
When $A \oplus B$is written in base two, the digit in the $2^k$'s place ($k \geq 0$) is $1$if exactly one of $A$and $B$is $1$, and $0$otherwise.
</li>

</ul>
For example, we have $3 \oplus 5 = 6$(in base two: $011 \oplus 101 = 110$).
    
<p>

</p>

</details>

<p>


Your objective is to make $A_i = i$for every $i$. Determine whether it is achievable. It can be proved that, under the Constraints of this problem, one can achieve the objective with at most $10^6$operations if it is achievable at all. Print such a sequence of operations.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N\leq 18$
</li>

<li>
$0\leq A_i \leq 2^N - 1$
</li>

<li>
$A_i\neq A_j$, if $i\neq j$
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
Input is given from Standard Input in the following format:
</p>

<div>

$N$$A_0$$A_1$$\ldots$$A_{2^N - 1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If it is possible to make $A_i = i$for every $i$, print `Yes`; otherwise, print `No`.
</p>

<p>
In the case of `Yes`, it should be followed by a sequence of operations that achieves the objective, in the following format:
</p>

<div>

$K$$x_1$$x_2$$\ldots$$x_K$
</div>

<p>
Here, $K$is a non-negative integer representing the number of operations, which must satisfy $0\leq K\leq 10^6$; $x_i$is an integer representing the $i$-th operation, which should be set as follows.
</p>

<ul>

<li>
If the $i$-th operation is Operation $+$, $x_i=-1$.
</li>

<li>
If the $i$-th operation is Operation $\oplus$, $x_i$should be the integer chosen in that operation.
</li>

</ul>

<p>
If there are multiple possible solutions, you may print any of them.
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
5 0 3 6 1 4 7 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
4
-1 6 -1 1

</div>

<p>
The sequence of operations above changes the sequence $A$as follows.
</p>

<ul>

<li>
Initially: $A = (5,0,3,6,1,4,7,2)$
</li>

<li>
Operation $+$: $A = (6,1,4,7,2,5,0,3)$
</li>

<li>
Operation $\oplus$($x = 6$)：$A = (0,7,2,1,4,3,6,5)$
</li>

<li>
Operation $+$: $A = (1,0,3,2,5,4,7,6)$
</li>

<li>
Operation $\oplus$($x = 1$)：$A = (0,1,2,3,4,5,6,7)$
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
2 5 4 3 6 1 0 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No

</div>

<p>
No sequence of operations achieves the objective.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

3
0 1 2 3 4 5 6 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

Yes
0


</div>

<p>
Performing zero operations achieves the objective. Whether an empty line is printed or not does not affect the verdict.
</p>

</section>

</div>

</span>

</span>

</div>
