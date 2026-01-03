
<div>

<span>

<span>

<p>
Score : $650$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<p>
Happy New Year! When it comes to indoor play on New Year's, it's sugoroku!
</p>

</blockquote>

<p>
There is a sugoroku board consisting of $N+1$squares: squares $0$, square $1$, $\dots$, square $N$.

There is an $M$-sided die (dice) that produces positive integers $A_1, A_2, \dots, A_M$with equal probability. Here, $A_1, A_2, \dots, A_M$are distinct.

Person $1$, person $2$, $\dots$, person $L$will play a game using this board. The game proceeds as follows:
</p>

<ul>

<li>
Initially, place $L$pieces, piece $1$, piece $2$, $\dots$, piece $L$, on square $0$.
</li>

<li>
Turns come around in numerical order starting with person $1$. Strictly speaking, after person $i$'s turn, the turn goes to person $(i \bmod L) + 1$. Each person performs the following operation on their turn:
<ul>

<li>
Let $i$be the number of the person whose turn it is. Roll the die. Let $x$be the square where piece $i$is located and $y$be the integer that came up on the die, and move piece $i$to square $\min(N, x+y)$.
</li>

</ul>

</li>

<li>
The first person to place their numbered piece on square $N$wins, and the other people lose.
</li>

</ul>

<p>
For $i =1,2,\dots,L$, find the probability, modulo $998244353$, that person $i$wins.
</p>

<details>

<summary>
What is probability $\text{mod }998244353$?
</summary>
It can be proved that the probability to be found is always a rational number.  
Also, under the constraints of this problem, when the value is expressed as $\frac{P}{Q}$using two coprime integers $P$and $Q$, it can be proved that there exists exactly one integer $R$that satisfies $R \times Q \equiv P\pmod{998244353}$and $0 \leq R \lt 998244353$. Find this $R$.


</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 2.5 \times 10^5$
</li>

<li>
$1 \leq M \leq N$
</li>

<li>
$2 \leq L \leq 2.5 \times 10^5$
</li>

<li>
$1 \leq A_1 \lt A_2 \lt \dots \lt A_M \leq N$
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

$N$$M$$L$$A_1$$A_2$$\dots$$A_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $L$lines. The $i$-th line should contain the probability that person $i$wins the game, computed modulo $998244353$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2 2 3
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

374341633
748683265
873463809

</div>

<p>
Person $1$wins with the probability $\frac{5}{8}$, person $2$wins with the probability $\frac{1}{4}$, and person $3$wins with the probability $\frac{1}{8}$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

100 2 4
20 26

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

164734081
939753473
943409153
946836353

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

123456 12 10
21994 29598 47718 59035 69293 73766 74148 76721 98917 104184 120533 122441

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

580013367
81975961
178650340
610261473
14826260
541995390
307779600
913805572
76177928
687491522

</div>

</section>

</div>

</span>

</span>

</div>
