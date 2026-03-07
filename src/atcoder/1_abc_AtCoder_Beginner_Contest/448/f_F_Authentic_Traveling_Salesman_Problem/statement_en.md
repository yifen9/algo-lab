
<div>

<span>

<span>

<p>
Score : $525$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$locations numbered $1$to $N$on a two-dimensional plane. Location $i$is at coordinates $(X_i, Y_i)$.

You will start from location $1$, visit every location exactly once, and return to location $1$.

Moving from location $i$to location $j$takes $\vert X_i - X_j \vert + \vert Y_i - Y_j \vert$seconds.

Output a route that visits all locations and returns to location $1$within $10^{10}$seconds of starting from location $1$. It is guaranteed that at least one such route exists under the given constraints.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 6 \times 10^4$
</li>

<li>
$0 \leq X_i \leq 2 \times 10^7$
</li>

<li>
$0 \leq Y_i \leq 2 \times 10^7$
</li>

<li>
$(X_i, Y_i) \neq (X_j, Y_j)$if $i \neq j$
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

$N$$X_1$$Y_1$$X_2$$Y_2$$\vdots$$X_N$$Y_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $p_i$be the $i$-th location visited $(1 \leq i \leq N)$, and output your answer in the following format.
</p>

<div>

$p_1$$p_2$$\dots$$p_N$
</div>

<p>
Your answer is considered correct if all of the following conditions are satisfied.
</p>

<ul>

<li>
$(p_1, p_2, \dots, p_N)$is a permutation of $(1, 2, \dots, N)$.
</li>

<li>
$p_1 = 1$
</li>

<li>
Letting $d(i, j)$be the number of seconds it takes to move from location $i$to location $j$, $\displaystyle \sum_{i=1}^N d(p_i, p_{(i \bmod N) + 1} ) \leq 10^{10}$.
</li>

</ul>

<p>
If there are multiple valid answers, any of them will be accepted.
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
0 6
3 5
2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1 3 2

</div>

<p>
$\displaystyle \sum_{i=1}^N d(p_i, p_{(i \bmod N) + 1}) = 4 + 2 + 4 = 10$, so the output satisfies the condition.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10
9706344 19786176
19341349 15565412
5711023 19068083
12521132 14054301
14767612 17088029
14961700 18526945
13801766 5740101
6581153 8643675
13176196 16586661
4086263 5172719

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1 5 2 6 4 7 9 8 3 10

</div>

</section>

</div>

</span>

</span>

</div>
