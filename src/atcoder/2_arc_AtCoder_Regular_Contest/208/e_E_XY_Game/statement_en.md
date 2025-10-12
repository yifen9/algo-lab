
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
You are given positive integers $N$, $X$, $Y$and a length-$N$integer sequence $A=(A_1,A_2,\ldots,A_N)$.
</p>

<p>
There are $N$piles of stones, and the $i$-th pile $(1\le i\le N)$has $A_i$stones.
</p>

<p>
Alice and Bob will play the following game using these piles:
</p>

<ul>

<li>
Starting with Alice, the two players take turns alternately.
</li>

<li>
In each turn, the player chooses one non-empty pile and removes one or two stones from that pile. However, the player cannot make a move such that the number of stones in that pile becomes a multiple of $X$or a multiple of $Y$after removing stones.
</li>

</ul>

<p>
The player who cannot make a move first loses.
</p>

<p>
Determine which player wins when both players play optimally.
</p>

<p>
You are given $T$test cases, solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le T \le 2\times 10^5$
</li>

<li>
$1\le N \le 2\times 10^5$
</li>

<li>
The sum of $N$over all test cases is at most $2\times 10^5$.
</li>

<li>
$1\le X < Y\le 10^9$
</li>

<li>
$1\le A_i \le 10^{18}$
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

$N$$X$$Y$$A_1$$A_2$$\ldots$$A_N$
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
For each test case, print `Alice`if Alice wins when both players play optimally, and `Bob`if Bob wins.
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
2 3 5
4 12
5 1 2
1 2 3 4 5
6 530 879
17031 42909 97721 34323 39597 26999

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Alice
Bob
Alice

</div>

<p>
Consider the first test case.
</p>

<p>
For example, the game proceeds as follows:
</p>

<ul>

<li>
Alice removes two stones from the first pile. The first pile has two stones remaining.
</li>

<li>
Bob removes one stone from the second pile. The second pile has eleven stones remaining.
</li>

<li>
Alice removes one stone from the first pile. The first pile has one stone remaining.
</li>

<li>
Bob cannot make a move, so Bob loses and Alice wins.
</li>

</ul>

<p>
In this test case, Alice always wins no matter how both players make their moves. Therefore, print `Alice`on the first line.
</p>

</section>

</div>

</span>

</span>

</div>
