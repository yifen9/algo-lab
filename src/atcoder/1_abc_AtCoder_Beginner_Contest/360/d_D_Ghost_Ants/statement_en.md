
<div>

<span>

<span>

<p>
Score : $350$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$ants on a number line, labeled $1$to $N$. Ant $i$$(1 \leq i \leq N)$starts at coordinate $X_i$and faces either a positive or negative direction. Initially, all ants are at distinct coordinates. The direction each ant is facing is represented by a binary string $S$of length $N$, where ant $i$is facing the negative direction if $S_i$is `0`and the positive direction if $S_i$is `1`.
</p>

<p>
Let the current time be $0$, and the ants move in their respective directions at a speed of $1$unit per unit time for $(T+0.1)$units of time until time $(T+0.1)$. If multiple ants reach the same coordinate, they pass through each other without changing direction or speed. After $(T+0.1)$units of time, all ants stop.
</p>

<p>
Find the number of pairs $(i, j)$such that $1 \leq i < j \leq N$and ants $i$and $j$pass each other from now before time $(T+0.1)$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 2 \times 10^{5}$
</li>

<li>
$1 \leq T \leq 10^{9}$
</li>

<li>
$S$is a string of length $N$consisting of `0`and `1`.
</li>

<li>
$-10^{9} \leq X_i \leq 10^{9}$$(1 \leq i \leq N)$
</li>

<li>
$X_i \neq X_j$$(1 \leq i < j \leq N)$
</li>

<li>
$N$, $T$, and $X_i$$(1 \leq i \leq N)$are integers.
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

$N$$T$$S$$X_1$$X_2$... $X_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

6 3
101010
-5 -1 0 1 2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

5

</div>

<p>
The following five pairs of ants pass each other:
</p>

<ul>

<li>
Ant $3$and ant $4$pass each other at time $0.5$.
</li>

<li>
Ant $5$and ant $6$pass each other at time $1$.
</li>

<li>
Ant $1$and ant $2$pass each other at time $2$.
</li>

<li>
Ant $3$and ant $6$pass each other at time $2$.
</li>

<li>
Ant $1$and ant $4$pass each other at time $3$.
</li>

</ul>

<p>
No other pairs of ants pass each other, so print $5$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

13 656320850
0100110011101
-900549713 -713494784 -713078652 -687818593 -517374932 -498415009 -472742091 -390030458 -379340552 -237481538 -44636942 352721061 695864366

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

14

</div>

</section>

</div>

</span>

</span>

</div>
