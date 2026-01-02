
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
There are $N$rabbits numbered $1$to $N$on a number line. Rabbit $i$is at coordinate $X_i$. Multiple rabbits may be at the same coordinate.

Each rabbit has a parameter called 
<strong>
jumping power
</strong>
, and rabbit $i$has jumping power $R_i$.

Now, all rabbits will jump exactly once. When a rabbit at coordinate $x$with jumping power $r$jumps, it moves to coordinate $x+r$or coordinate $x-r$.

If you can freely choose which coordinate each rabbit jumps to, find the maximum possible number of distinct coordinates where rabbits are present after all rabbits have jumped.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$-10^9 \leq X_i \leq 10^9$
</li>

<li>
$1 \leq R_i \leq 10^9$
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

$N$$X_1$$R_1$$X_2$$R_2$$\vdots$$X_N$$R_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the maximum possible number of distinct coordinates where rabbits are present after jumping.
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
4 1
2 3
4 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3

</div>

<p>
If each rabbit moves as shown below, it is possible to achieve $3$as the number of distinct coordinates where rabbits are present after jumping, and this is the maximum possible.
</p>

<ul>

<li>
Rabbit $1$moves to $4 - 1 = 3$.
</li>

<li>
Rabbit $2$moves to $2 + 3 = 5$.
</li>

<li>
Rabbit $3$moves to $4 - 5 = -1$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6
2 1
3 2
6 1
5 2
4 3
4 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

4

</div>

<p>
If each rabbit moves as shown below, it is possible to achieve $4$as the number of distinct coordinates where rabbits are present after jumping, and this is the maximum possible.
</p>

<ul>

<li>
Rabbit $1$moves to $2 - 1 = 1$.
</li>

<li>
Rabbit $2$moves to $3 + 2 = 5$.
</li>

<li>
Rabbit $3$moves to $6 + 1 = 7$.
</li>

<li>
Rabbit $4$moves to $5 + 2 = 7$.
</li>

<li>
Rabbit $5$moves to $4 - 3 = 1$.
</li>

<li>
Rabbit $6$moves to $4 - 1 = 3$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10
1000000000 1000000000
1000000000 1
-1000000000 1000000000
-1000000000 1
0 1
2 1
1 2
4 1
3 2
4 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

9

</div>

</section>

</div>

</span>

</span>

</div>
