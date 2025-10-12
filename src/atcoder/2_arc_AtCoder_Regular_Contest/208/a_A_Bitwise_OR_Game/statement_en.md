
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

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
In each turn, the player chooses one non-empty pile and removes one or more stones from that pile. However, the player cannot make a move that changes the bitwise $\mathrm{OR}$of the numbers of stones of all piles.
</li>

</ul>

<p>
The player who cannot make a move first loses.
</p>

<p>
Determine which player wins when both players play optimally.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

<details>

<summary>
What is bitwise $\mathrm{OR}$?
    
</summary>

<p>
The bitwise $\mathrm{OR}$of non-negative integers $A$and $B$, $A\ \mathrm{OR}\ B$, is defined as follows:
        
</p>

<ul>

<li>
When $A\ \mathrm{OR}\ B$is written in binary, the digit in the $2^k$place ($k \geq 0$) is $1$if at least one of the digits in the $2^k$place of $A$and $B$written in binary is $1$, and $0$otherwise.
</li>

</ul>
For example, $3\ \mathrm{OR}\ 5 = 7$(in binary: $011\ \mathrm{OR}\ 101 = 111$).

In general, the bitwise $\mathrm{OR}$of $k$non-negative integers $p_1, p_2, p_3, \dots, p_k$is defined as $(\dots ((p_1\ \mathrm{OR}\ p_2)\ \mathrm{OR}\ p_3)\ \mathrm{OR}\ \dots\ \mathrm{OR}\ p_k)$, and it can be proved that this is independent of the order of $p_1, p_2, p_3, \dots p_k$.  
    
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
$1\le T\le 10^5$
</li>

<li>
$2\le N \le 2\times 10^5$
</li>

<li>
The sum of $N$over all test cases is at most $2\times 10^5$.
</li>

<li>
$1\le A_i \le 10^9$
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

$N$$A_1$$A_2$$\ldots$$A_N$
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

4
3
3 4 6
3
7 7 7
3
9 3 5
10
1 9 1 3 7 9 10 9 7 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Alice
Bob
Bob
Alice

</div>

<p>
Consider the first test case.
</p>

<p>
Initially, the bitwise $\mathrm{OR}$of the numbers of stones of all piles is $3\ \mathrm{OR}\ 4\ \mathrm{OR}\ 6=7$.
</p>

<p>
The moves Alice can make are as follows:
</p>

<ul>

<li>
Remove two stones from the first pile.
</li>

<li>
Remove one or more stones from the second pile.
</li>

<li>
Remove one or more stones from the third pile.
</li>

</ul>

<p>
For example, if Alice removes one stone from the first pile, the bitwise $\mathrm{OR}$of the numbers of stones of all piles becomes $2\ \mathrm{OR}\ 4\ \mathrm{OR}\ 6=6$. Therefore, Alice cannot make the move of removing one stone from the first pile.
</p>

<p>
If Alice removes six stones from the third pile, Bob cannot make any move in the next turn. Therefore, the winner when both players play optimally is Alice.
</p>

</section>

</div>

</span>

</span>

</div>
