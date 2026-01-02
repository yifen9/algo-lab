
<div>

<span>

<span>

<p>
Score : $200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$birds of $M$types flying in the sky.

The bird types are numbered $1,2,\dots,M$.

The $N$birds are numbered $1,2,\dots,N$, and bird $i$is of type $A_i$and has size $B_i$.
</p>

<p>
For every $k=1,2,\dots,M$, find the average size of the flying birds of type $k$.

It is guaranteed that for every $k=1,2,\dots,M$, there is at least one bird of type $k$flying.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le M \le N \le 100$
</li>

<li>
$1 \le A_i \le M$
</li>

<li>
$1 \le B_i \le 100$
</li>

<li>
There exists at least one bird of type $k$( $1 \le k \le M$).
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

$N$$M$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_N$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $M$lines.

The $k$-th line ( $1 \le k \le M$) should contain the average size of birds of type $k$.

Your answer will be considered correct if the absolute or relative error from the true value is at most $10^{-5}$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

10 5
4 92
1 16
3 77
4 99
2 89
3 8
1 40
5 56
1 40
4 77

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

32.00000000000000000000
89.00000000000000000000
42.50000000000000000000
89.33333333333333333333
56.00000000000000000000

</div>

<ul>

<li>
The average size of birds of type $1$is $(16+40+40)/3 = 32$.
</li>

<li>
The average size of birds of type $2$is $89$.
</li>

<li>
The average size of birds of type $3$is $(77+8)/2 = 42.5$.
</li>

<li>
The average size of birds of type $4$is $(92+99+77)/3 \approx 89.3333$.
</li>

<li>
The average size of birds of type $5$is $56$.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
