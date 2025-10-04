
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$versions of a certain OS, numbered $1,2,\dots,N$in chronological order.

There are $N$PCs, and initially the OS version of the $i$-th PC is $i$.
</p>

<p>
Perform $Q$operations in order. The $i$-th operation is as follows:
</p>

<ul>

<li>
Upgrade all PCs whose current OS version is $X_i$or earlier to version $Y_i(>X_i)$. Then, print the number of PCs upgraded in this operation.
</li>

</ul>

<p>
Note that for $i<Q$, the upgrades from the $i$-th operation are performed before proceeding to the $(i+1)$-th operation.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
All input values are integers.
</li>

<li>
$2 \le N \le 10^6$
</li>

<li>
$1 \le Q \le 2 \times 10^5$
</li>

<li>
$1 \le X_i < Y_i \le N$
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

$N$$Q$$X_1$$Y_1$$X_2$$Y_2$$\vdots$$X_Q$$Y_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.

The $i$-th line should contain the number of PCs upgraded in the $i$-th operation.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

8 5
2 6
3 5
1 7
5 7
7 8

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
1
0
3
7

</div>

<p>
This input contains five operations.
</p>

<ul>

<li>
Initially, the versions of the eight PCs are $1,2,3,4,5,6,7,8$.
</li>

<li>
In the first operation, PCs with version $2$or earlier are upgraded to version $6$.
<ul>

<li>
This operation upgrades two PCs, and the versions of the PCs become $6,6,3,4,5,6,7,8$.
</li>

</ul>

</li>

<li>
In the second operation, PCs with version $3$or earlier are upgraded to version $5$.
<ul>

<li>
This operation upgrades one PC, and the versions of the PCs become $6,6,5,4,5,6,7,8$.
</li>

</ul>

</li>

<li>
In the third operation, PCs with version $1$or earlier are upgraded to version $7$.
<ul>

<li>
This operation upgrades zero PCs, and the versions of the PCs become $6,6,5,4,5,6,7,8$.
</li>

</ul>

</li>

<li>
In the fourth operation, PCs with version $5$or earlier are upgraded to version $7$.
<ul>

<li>
This operation upgrades three PCs, and the versions of the PCs become $6,6,7,7,7,6,7,8$.
</li>

</ul>

</li>

<li>
In the fifth operation, PCs with version $7$or earlier are upgraded to version $8$.
<ul>

<li>
This operation upgrades seven PCs, and the versions of the PCs become $8,8,8,8,8,8,8,8$.
</li>

</ul>

</li>

</ul>

</section>

</div>

</span>

</span>

</div>
