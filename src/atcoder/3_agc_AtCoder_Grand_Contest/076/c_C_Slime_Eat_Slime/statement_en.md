
<div>

<span>

<span>

<p>
Score : $1200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$slimes numbered from $1$to $N$.
The color of each slime is represented by an integer between $0$and $2K$(inclusive), and the color of slime $i$is $C_i$.
</p>

<p>
Currently, $M$pairs of slimes are in a (bidirectional) friendship. Specifically, slimes $A_i$and $B_i$are friends ($1 \leq i \leq M$).
Here, it is guaranteed that for any two slimes, one can reach the other by following friendship relations.
</p>

<p>
You can perform the following operation:
</p>

<ul>

<li>
First, choose a pair of slimes $(u,v)$that satisfies both of the following conditions:
<ul>

<li>
Slimes $u$and $v$are in a friendship.
</li>

<li>
$(C_u - C_v) \bmod (2K+1) \geq K+1$(here, the result of $x \bmod y$is always in the range $[0,y-1]$).
</li>

</ul>

</li>

<li>
Then, let slime $u$eat slime $v$.
Slime $v$disappears from the field.
Also, all slimes except $u$that were in a friendship with slime $v$become friends with slime $u$(if they were already friends with slime $u$, nothing happens).
</li>

</ul>

<p>
Determine whether it is possible to leave only slime $1$on the field by repeating the operation appropriately.
</p>

<p>
Solve $T$cases for one input.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq 125000$
</li>

<li>
$2 \leq N \leq 250000$
</li>

<li>
$N-1 \leq M \leq 250000$
</li>

<li>
$1 \leq K \leq N$
</li>

<li>
$0 \leq C_i \leq 2K$
</li>

<li>
$1 \leq A_i < B_i \leq N$
</li>

<li>
$(A_i,B_i) \neq (A_j,B_j)$($i \neq j$)
</li>

<li>
For any two slimes, one can reach the other by following friendship relations.
</li>

<li>
The sum of $N$over the $T$cases is at most $250000$.
</li>

<li>
The sum of $M$over the $T$cases is at most $250000$.
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
Each test case is given in the following format:
</p>

<div>

$N$$M$$K$$C_1$$C_2$$\cdots$$C_N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_M$$B_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines.
The $i$-th line should contain `Yes`if it is possible to leave only slime $1$on the field for the $i$-th case, and `No`otherwise.
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
2 1 1
0 0
1 2
3 2 1
0 2 1
1 2
2 3
6 6 1
0 0 1 2 1 0
1 2
2 3
3 4
4 5
5 6
1 6
5 4 2
2 4 3 2 1
1 2
2 4
2 5
3 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

No
Yes
No
No

</div>

<p>
In the first test case, no operation can be performed.
</p>

<p>
In the second test case, it is possible to leave only slime $1$on the field by the following procedure:
</p>

<ul>

<li>
Choose $(u,v)=(3,2)$and let slime $3$eat slime $2$. Slime $2$disappears, and slimes $1$and $3$become friends.
</li>

<li>
Choose $(u,v)=(1,3)$and let slime $1$eat slime $3$. Slime $3$disappears.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
