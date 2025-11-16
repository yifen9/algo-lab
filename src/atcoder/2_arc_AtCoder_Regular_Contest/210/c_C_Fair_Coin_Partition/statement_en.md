
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
There are $N$types of coins. For $0\leq i\leq N-1$, the $(1+i)$-th type of coin has a value of $10^{i}$, and you possess $A_i$of these coins.
</p>

<p>
You have decided to distribute these coins to $M$people. However, the total value of coins distributed to each person must be equal. It is allowed to have coins that are not distributed.
</p>

<p>
Find the maximum possible total value of coins distributed to each person.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq T\leq 10^5$
</li>

<li>
$1\leq N\leq 2\times 10^5$
</li>

<li>
$1\leq M\leq 10^9$
</li>

<li>
$0\leq A_i\leq 10^9$
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$M$$A_0$$A_1$$\ldots$$A_{N-1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the maximum possible total value of coins distributed to each person.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5
3 1
123 456 789
3 1000
123 456 789
2 3
6 14
2 3
11 14
30 4
15 9 2 66 23 2 4 1 1 32 4 80 9 10 47 14 8 7 3 16 2 39 77 4 4 2 38 64 1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

83583
0
42
50
19401302040124704218001124023

</div>

<ul>

<li>
For the first test case, if all coins are distributed to one person, the total value of coins distributed to each person is $123\times 10^0+456\times 10^1+789\times 10^2=83583$.
</li>

<li>
For the second test case, there is no choice but to distribute $0$coins to everyone.
</li>

<li>
For the third test case, the total value of coins distributed to each person can be made $42$as follows:
<ul>

<li>
To the $1$-st person, distribute $2$coins of value $10^0$and $4$coins of value $10^1$.
</li>

<li>
To the $2$-nd person, distribute $2$coins of value $10^0$and $4$coins of value $10^1$.
</li>

<li>
To the $3$-rd person, distribute $2$coins of value $10^0$and $4$coins of value $10^1$.
</li>

</ul>

</li>

<li>
For the fourth test case, the total value of coins distributed to each person can be made $50$as follows:
<ul>

<li>
To the $1$-st person, distribute $0$coins of value $10^0$and $5$coins of value $10^1$.
</li>

<li>
To the $2$-nd person, distribute $0$coins of value $10^0$and $5$coins of value $10^1$.
</li>

<li>
To the $3$-rd person, distribute $10$coins of value $10^0$and $4$coins of value $10^1$.
</li>

</ul>

</li>

</ul>

</section>

</div>

</span>

</span>

</div>
