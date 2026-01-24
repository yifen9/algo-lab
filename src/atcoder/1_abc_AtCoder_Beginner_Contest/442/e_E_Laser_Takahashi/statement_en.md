
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$monsters on a two-dimensional plane.
The monsters are numbered from $1$to $N$, and the coordinates of monster $i$are $(X_i,Y_i)$.
Here, $(X_i,Y_i) \neq (0,0)$.
(Each monster can be regarded as a stationary point. That is, monsters have no size.)
</p>

<p>
Takahashi is standing at the origin of this plane.
A powerful laser is always emitted from his eyes, instantly destroying monsters in the direction he is facing.
If multiple monsters exist in the direction he is facing, all of them are instantly destroyed.
</p>

<p>
Aoki is conducting $Q$
<strong>
independent
</strong>
thought experiments.
The $j$-th thought experiment is as follows:
</p>

<ul>

<li>
Initially, Takahashi is facing the direction toward monster $A_j$. From now on, Takahashi will rotate 
<strong>
clockwise
</strong>
and stop the moment he faces the direction toward monster $B_j$.
Here, how many monsters in total (including monsters $A_j$and $B_j$) will be destroyed? If monsters $A_j$and $B_j$exist in the same direction from the origin, Takahashi does not rotate at all.
</li>

</ul>

<p>
Find the answer to each thought experiment.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\leq N \leq 2\times 10^5$
</li>

<li>
$1\leq Q \leq 2\times 10^5$
</li>

<li>
$-10^9\leq X_i,Y_i \leq 10^9$
</li>

<li>
$(X_i,Y_i)\neq (0,0)$
</li>

<li>
$1\leq A_j,B_j\leq N$
</li>

<li>
$A_j\neq B_j$
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

$N$$Q$$X_1$$Y_1$$X_2$$Y_2$$\vdots$$X_N$$Y_N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_Q$$B_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.
The $j$-th line $(1\leq j \leq Q)$should contain the answer to the $j$-th thought experiment.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 4
0 1
1 -2
1 0
-2 0
3 0
4 1
1 4
5 4
3 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
5
4
2

</div>

<p>

<img src="https://img.atcoder.jp/abc442/ec8e15d827e64ccfdae57c4bad47cebc.png">

</img>

</p>

<ul>

<li>
$1$-st thought experiment: Initially, Takahashi is facing the direction toward monster $4$(at this time, monster $4$is destroyed).
From here, he continues to rotate clockwise and stops the moment he faces the direction toward monster $1$(at this time, monster $1$is destroyed).
Since he does not face the direction toward any other monsters, the answer is $2$.
</li>

<li>
$2$-nd thought experiment: Initially, Takahashi is facing the direction toward monster $1$(at this time, monster $1$is destroyed).
From here, as he continues to rotate clockwise, he faces the direction toward monsters $3$and $5$along the way, so they are destroyed.
As he continues to rotate further, he faces the direction toward monster $2$along the way, so it is destroyed.
Finally, he stops the moment he faces the direction toward monster $4$(at this time, monster $4$is destroyed).
Therefore, the answer is $5$.
</li>

<li>
$3$-rd thought experiment: Monsters $3, 5, 2, 4$are destroyed, so the answer is $4$.
</li>

<li>
$4$-th thought experiment: Monsters $3, 5$are destroyed, so the answer is $2$.
Note that since monsters $3$and $5$exist in the same direction from the origin, Takahashi does not rotate at all.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2 1
1 2
1 2
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

2

</div>

<p>
Multiple monsters may exist at the same coordinates.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

8 10
-84 -60
-100 8
77 55
-14 -10
50 -4
-63 -45
26 -17
-7 -5
3 7
2 4
8 4
8 4
7 1
1 7
6 3
4 7
4 5
2 6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

3
8
4
4
5
8
6
8
7
8

</div>

</section>

</div>

</span>

</span>

</div>
