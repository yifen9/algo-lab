
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
You are given strings $s$and $t$of length $N$consisting of `0`and `1`.
Determine whether it is possible to make $s$match $t$by performing the following operation at least $0$and at most $N+1$times, and if possible, show one such sequence of operations.
</p>

<p>
Operation: Perform the following in order.
</p>

<ol>

<li>
Choose integers $a$and $b$satisfying $1 \le a,b \le N$and $|a-b|=1$
</li>

<li>
Append the $a$-th character from the beginning of $s$to the end of $s$
</li>

<li>
Remove the $b$-th character from the beginning of $s$and concatenate the remaining characters in their original order
</li>

</ol>

<p>
You are given $T$test cases; find the answer for each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 10^{5}$
</li>

<li>
$2 \le N \le 2 \times 10^{5}$
</li>

<li>
$s$and $t$are strings of length $N$consisting of `0`and `1`.
</li>

<li>
The sum of $N$over all test cases is at most $2 \times 10^{5}$.
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

$N$$s$$t$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answers for the given test cases in the order they are given.
If it is impossible to make $s$match $t$by performing the operation at least $0$and at most $N+1$times, print `-1`.
If possible, first print the number of operations $K$, and on the $j$-th of the following $K$lines, print the two integers $a_j$and $b_j$chosen in the $j$-th operation, separated by a space.
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
00101
00010
2
01
01
2
00
11

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
2 3
0
-1

</div>

<p>
In the first test case, $s$is `00101`and $t$is `00010`.
</p>

<ul>

<li>
By choosing $2$and $3$as $a$and $b$, appending the $2$-nd character `0`to the end of $s$, and then removing the $3$-rd character, we can make $s$and $t$match.
</li>

<li>
Note that the integers $a$and $b$chosen in the operation must satisfy $|a-b|=1$.
</li>

</ul>

<p>
In the second test case, $s$and $t$can be made to match with zero operations.
</p>

<p>
In the third test case, no matter how the operations are performed, $s$and $t$cannot be made to match.
</p>

</section>

</div>

</span>

</span>

</div>
