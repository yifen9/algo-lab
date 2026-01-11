
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$people numbered $1,2,\ldots,N$. For $i\neq j$, the intimacy between persons $i$and $j$is $A_{i,j}$.
</p>

<p>
For each of the $N$people, assign room $X$or room $Y$. Each of the $N$people moves to their assigned room. It is acceptable if there is an empty room.
</p>

<p>
Person $i$is in a 
<strong>
good state
</strong>
if the following is satisfied:
</p>

<blockquote>

<p>
(Sum of intimacy with person $i$of all people in the same room as person $i$) $\geq$(Sum of intimacy with person $i$of all people in a different room from person $i$).
</p>

</blockquote>

<p>
Output one assignment of rooms such that all $N$people are in a good state.
</p>

<p>
It can be proved that such an assignment always exists.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 50$
</li>

<li>
$-50 \leq A_{i,j} \leq 50$
</li>

<li>
$A_{i,j} = A_{j,i}$
</li>

<li>
$A_{i,i}=0$
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

$N$$A_{1,1}$$A_{1,2}$$\cdots$$A_{1,N}$$A_{2,1}$$A_{2,2}$$\cdots$$A_{2,N}$$\vdots$$A_{N,1}$$A_{N,2}$$\cdots$$A_{N,N}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output one assignment that satisfies the condition. If there are multiple solutions, you may output any of them.
Represent the assignment by a string $S$of length $N$. If person $i$is assigned to room $X$, the $i$-th character of $S$should be `X`; if assigned to room $Y$, the $i$-th character of $S$should be `Y`.
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
0 4 -2 -1
4 0 -3 -5
-2 -3 0 2
-1 -5 2 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

XXYY

</div>

<p>
Suppose persons $1,2$are assigned to room $X$and persons $3,4$are assigned to room $Y$.
</p>

<p>
For person $1$, the sum of intimacy with people in the same room (person $2$) is $4$, and the sum of intimacy with people in different rooms (persons $3$and $4$) is $(-2)+(-1)=-3$, so they are in a good state.
</p>

<p>
All other people are also in a good state, so this assignment satisfies the condition.
</p>

<p>
Outputting `YYXX`is also correct.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
0 0 0
0 0 0
0 0 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

XXX

</div>

<p>
It is acceptable if there is an empty room.
</p>

</section>

</div>

</span>

</span>

</div>
