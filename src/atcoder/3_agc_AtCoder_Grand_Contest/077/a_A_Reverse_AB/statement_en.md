
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
You are given strings $X$and $Y$of length $N$consisting of `A`and `B`. Let $X_i$denote the $i$-th character of $X$.
</p>

<p>
Determine whether it is possible to make $X$equal to $Y$by performing the following operation between $0$and $\left\lfloor \frac{N}{2} \right\rfloor$times, inclusive.
</p>

<ul>

<li>
Choose a pair of integers $(l, r)$such that $1\leq l < r \leq N$, $X_l=$`A`, and $X_r=$`B`. Reverse the elements of $X$from the $l$-th to the $r$-th position. Here, "reversing the elements of $X$from the $l$-th to the $r$-th position" means simultaneously replacing $X_l,X_{l+1},\ldots,X_{r-1},X_r$with $X_r,X_{r-1},\ldots,X_{l+1},X_l$.
</li>

</ul>

<p>
If it is possible to make $X$equal to $Y$, output one such sequence of operations.
</p>

<p>
$T$test cases are given; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq  2.5\times 10^5$
</li>

<li>
$2 \leq N \leq 5\times 10^5$
</li>

<li>
The sum of $N$over all test cases is at most $5\times 10^5$.
</li>

<li>
$X$and $Y$are strings of length $N$consisting of `A`and `B`.
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
Each test case is given in the following format:
</p>

<div>

$N$$X$$Y$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for $\mathrm{case}_1,\mathrm{case}_2,\ldots,\mathrm{case}_T$in this order in the following format.
</p>

<p>
If it is impossible to make $X$equal to $Y$using between $0$and $\left\lfloor \frac{N}{2} \right\rfloor$operations, inclusive, output `No`.
</p>

<p>
If it is possible, output a sequence of operations in the following format:
</p>

<div>

Yes
$K$$l_1$$r_1$$l_2$$r_2$$\vdots$$l_K$$r_K$
</div>

<p>
Here $K$is the number of operations, and $l_i, r_i$are the integers $l, r$chosen in the $i$-th operation. These must satisfy the following:
</p>

<ul>

<li>
$0 \leq K \leq \left\lfloor \frac{N}{2} \right\rfloor$
</li>

<li>
$1 \leq l_i < r_i \leq N$
</li>

</ul>

<p>
If there are multiple valid sequences of operations, any of them will be accepted.
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
5
ABAAB
ABBAA
4
AAAA
BBBB
10
BABBAABBAA
BBBBAAABAA

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
1
3 5
No
Yes
3
2 7
4 6
3 5

</div>

<p>
In the first test case, $X_3=$`A`and $X_5=$`B`, so we can perform the operation of reversing the elements of $X$from the $3$-rd to the $5$-th position. After this operation, $X$is `ABBAA`, which equals $Y$.
</p>

<p>
In the second test case, it is impossible to make $X$equal to $Y$regardless of the operations performed.
</p>

</section>

</div>

</span>

</span>

</div>
