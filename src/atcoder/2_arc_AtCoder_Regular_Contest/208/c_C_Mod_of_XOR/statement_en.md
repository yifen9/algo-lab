
<div>

<span>

<span>

<p>
Score : $700$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given positive integers $C$and $X$that are less than $2^{30}$.
</p>

<p>
Determine whether there exists a positive integer $n$that satisfies all of the following conditions, and if it exists, find one such $n$.
</p>

<ul>

<li>
$1\le n < 2^{60}$
</li>

<li>
$(n \oplus C) \bmod n=X$
</li>

</ul>

<p>
Here, $n \oplus C$denotes the bitwise $\mathrm{XOR}$of $n$and $C$.
</p>

<p>
You are given $T$test cases, solve each of them.
</p>

<details>

<summary>
What is bitwise $\mathrm{XOR}$?
    
</summary>

<p>
The bitwise $\mathrm{XOR}$of non-negative integers $X$and $Y$, $X \oplus Y$, is defined as follows:
        
</p>

<ul>

<li>
When $X \oplus Y$is written in binary, the digit in the $2^k$place ($k \geq 0$) is $1$if exactly one of the digits in the $2^k$place of $X$and $Y$written in binary is $1$, and $0$otherwise.
</li>

</ul>
For example, $3 \oplus 5 = 6$(in binary: $011 \oplus 101 = 110$).


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
$1\le T\le 2\times 10^5$
</li>

<li>
$1\le C,X < 2^{30}$
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$C$$X$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for each test case in order, separated by newlines.
</p>

<p>
For each test case, if there does not exist an $n$that satisfies all conditions, print `-1`.
</p>

<p>
Otherwise, print $n$that satisfies all conditions.
</p>

<p>
If there are multiple $n$that satisfy all conditions, any of them will be accepted.
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
10 6
2 3
777 153

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

7
-1
208

</div>

<p>
Consider the first test case.
</p>

<p>
$n=7$satisfies all conditions because $(n\oplus C) \bmod n = (7 \oplus 10) \bmod 7 = 13\bmod 7 = 6=X$. Therefore, printing $7$on the first line will be accepted.
</p>

<p>
Other than this, printing $n=12,18,19$etc. will also be accepted.
</p>

</section>

</div>

</span>

</span>

</div>
