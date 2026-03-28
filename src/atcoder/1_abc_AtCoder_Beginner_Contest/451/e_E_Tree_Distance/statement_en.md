
<div>

<span>

<span>

<p>
Score : $475$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Determine whether there exists a weighted undirected tree with $N$vertices satisfying the following condition.
</p>

<ul>

<li>
For any two integers $i$and $j$with $1 \le i \lt j \le N$, the distance between vertices $i$and $j$is $A_{i,j}$.
</li>

</ul>

<p>
Here, the distance between vertices $i$and $j$is defined as the sum of the weights of the edges on the unique simple path connecting these two vertices.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \le N \le 3000$
</li>

<li>
$1 \le A_{i,j} \le 9999$
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

$N$$A_{1, 2}$$A_{1, 3}$$\ldots$$A_{1, N}$$A_{2, 3}$$\ldots$$A_{2, N}$$\vdots$$A_{N-1,N}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If a tree satisfying the condition exists, output `Yes`; otherwise, output `No`.
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
2 5 4
3 2
5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes

</div>

<p>
For example, the tree with the following edges satisfies the condition.
</p>

<ul>

<li>
Edge $(1, 2)$has weight $2$.
</li>

<li>
Edge $(2, 3)$has weight $3$.
</li>

<li>
Edge $(2, 4)$has weight $2$.
</li>

</ul>

<p>
Thus, output `Yes`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4
2 5 4
3 2
6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No

</div>

<p>
No tree satisfying the condition exists. Thus, output `No`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10
1039 1802 3781 231 5828 1944 392 262 1481
763 2742 1270 4789 905 1431 1301 442
1979 2033 5552 142 2194 2064 1205
4012 7531 2121 4173 4043 3184
6059 2175 161 493 1712
5694 6220 6090 5231
2336 2206 1347
654 1873
1743

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

Yes

</div>

</section>

</div>

</span>

</span>

</div>
