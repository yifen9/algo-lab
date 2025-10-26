
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
You are given a positive integer $N$.

Output one pair of non-negative integer sequences $P=(P_1, P_2, \dots,P_N), A=(A_1, A_2, \dots,A_N)$that satisfies all of the following conditions:
</p>

<ul>

<li>
$0 \leq P_i < 2^{30}~(1 \leq i \leq N)$
</li>

<li>
$0 \leq A_i < 2^{30}~(1 \leq i \leq N)$
</li>

<li>
The length of a longest strictly increasing subsequence of $(P_1~\mathrm{OR}~A_i, P_2~\mathrm{OR}~A_i, \dots, P_N~\mathrm{OR}~A_i)$is $i$. $(1 \leq i \leq N)$
<ul>

<li>
$\mathrm{OR}$denotes the bitwise $\mathrm{OR}$operation.
</li>

</ul>

</li>

</ul>

<p>
It can be proved that under the constraints of this problem, there exists at least one pair $P, A$that satisfies the conditions.
</p>

<p>
Solve $T$test cases per input.
</p>

<details>

<summary>
What is bitwise $\mathrm{OR}$?
    
</summary>

<p>
The bitwise $\mathrm{OR}$of non-negative integers $A, B$, denoted $A\ \mathrm{OR}\ B$, is defined as follows:
        
</p>

<ul>

<li>
When $A\ \mathrm{OR}\ B$is written in binary, the digit at position $2^k$($k \geq 0$) is $1$if at least one of the digits at position $2^k$in the binary representations of $A$and $B$is $1$, and $0$otherwise.
</li>

</ul>
For example, $3\ \mathrm{OR}\ 5 = 7$(in binary: $011\ \mathrm{OR}\ 101 = 111$).


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
$1 \leq T$
</li>

<li>
$1 \leq N \leq 1024$
</li>

<li>
For test cases in a single input, the sum of $N$is at most $200000$.  
</li>

<li>
For test cases in a single input, the sum of $N^2$is at most $1024^2$.  
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each case is given in the following format:
</p>

<div>

$N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output a solution for $\mathrm{case}_1, \mathrm{case}_2, \dots, \mathrm{case}_T$in this order.
</p>

<p>
For each case, output the answer in the following format:
</p>

<div>

$P_1$$P_2$$\ldots$$P_N$$A_1$$A_2$$\ldots$$A_N$
</div>

<p>
If there are multiple solutions, any of them will be considered correct.
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
3
8
1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3 14 5
13 2 10
6 902 909 186 684 219 471 248
1023 249 64 0 264 768 778 794
2025
1026

</div>

<p>
For the first test case, the sample output is $P = (3, 14, 5), A = (13, 2, 10)$.
</p>

<ul>

<li>
One longest strictly increasing subsequence of $(3~\mathrm{OR}~13, 14~\mathrm{OR}~13, 5~\mathrm{OR}~13) = (15, 15, 13)$is $(13)$, whose length is $1$.
</li>

<li>
One longest strictly increasing subsequence of $(3~\mathrm{OR}~2, 14~\mathrm{OR}~2, 5~\mathrm{OR}~2) = (3, 14, 7)$is $(3, 7)$, whose length is $2$.
</li>

<li>
One longest strictly increasing subsequence of $(3~\mathrm{OR}~10, 14~\mathrm{OR}~10, 5~\mathrm{OR}~10) = (11, 14, 15)$is $(11, 14, 15)$, whose length is $3$.
</li>

</ul>

<p>
From the above, it can be confirmed that $P = (3, 14, 5), A = (13, 2, 10)$satisfies the conditions.
</p>

</section>

</div>

</span>

</span>

</div>
