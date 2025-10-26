
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
You are given integer sequences $A=(A_1,A_2,\dots,A_N),\; B=(B_1,B_2,\dots,B_N)$of length $N$consisting of $0$and $1$.
Let $A[i,j]$denote the contiguous subsequence from the $i$-th through $j$-th elements of sequence $A$. If $i>j$, $A[i,j]$is a sequence of length $0$.
You can perform the following operation on $A$at most $\lfloor\frac{N}{2}\rfloor$times:
</p>

<ul>

<li>
Choose four integers $a,b,c,d$that satisfy the following three conditions: 
<ul>

<li>
$1 \leq a \leq b < c \leq d \leq N$
</li>

<li>
$b-a=d-c$
</li>

<li>
$\sum_{i=a}^{b}{A_i}=\sum_{i=c}^{d}{A_i}$
</li>

</ul>

</li>

<li>
Swap $A[a,b]$and $A[c,d]$. More precisely, replace $A$with the concatenation of $A[1,a-1]$, $A[c,d]$, $A[b+1,c-1]$, $A[a,b]$, $A[d+1,N]$in this order. 
</li>

</ul>

<p>
Determine whether it is possible to make $A$match $B$, and if possible, construct one sequence of operations.
</p>

<p>
Solve $T$test cases per input.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq 25000$
</li>

<li>
$2 \leq N \leq 2 \times 10^5$
</li>

<li>
$0 \leq A_i \leq 1$
</li>

<li>
$0 \leq B_i \leq 1$
</li>

<li>
The sum of $N$over all test cases is at most $2\times 10^5$.
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

$T$$case_1$$case_2$$\vdots$$case_T$
</div>

<p>
Each case is given in the following format:
</p>

<div>

$N$$A_1$$A_2$$\dots$$A_N$$B_1$$B_2$$\dots$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer in the following format:
</p>

<div>

$output_1$$output_2$$\vdots$$output_T$
</div>

<p>
Here, $output_t$represents the output for the $t$-th test case.

For each case, if you can make $A$match $B$, let $K$be the number of operations required and $(a_k,b_k,c_k,d_k)$be the values chosen in the $k$-th operation, then output in the following format:
</p>

<div>

Yes
$K$$a_1$$b_1$$c_1$$d_1$$a_2$$b_2$$c_2$$d_2$$\vdots$$a_K$$b_K$$c_K$$d_K$
</div>

<p>
If it is impossible to make $A$match $B$, output `No`.
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
8
1 0 0 1 0 1 0 1
0 0 1 1 1 0 1 0
2
0 0
1 0
3
1 1 1
1 1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
2
3 4 6 7
1 4 5 8
No
Yes
0

</div>

<p>
In the first test case, $A$is initially $(1,0,0,1,0,1,0,1)$.

Performing the operation with $(a,b,c,d)=(3,4,6,7)$changes $A$to $(1,0,1,0,0,0,1,1)$.

Then, performing the operation with $(a,b,c,d)=(1,4,5,8)$changes $A$to $(0,0,1,1,1,0,1,0)$, which matches $B$.

In the second test case, it is impossible to make $A$match $B$.

In the third test case, $A$already matches $B$from the beginning.
</p>

</section>

</div>

</span>

</span>

</div>
