
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
You are given a tree $T$with $N$vertices. The vertices are numbered from $0$to $N-1$, and the $i$-th edge $(1\le i\le N-1)$bidirectionally connects vertices $u_i$and $v_i$. (Note that vertex numbers are 0-indexed and edge numbers are 1-indexed.)
</p>

<p>
For a pair of integers $(i,j)$where $0 \leq i,j < N$, define $f(i,j)$as follows:
</p>

<ul>

<li>
The vertex number of the vertex with the smallest number among the vertices 
<strong>
not included
</strong>
in the path from vertex $i$to vertex $j$in tree $T$.
<ul>

<li>
Here, if the path from vertex $i$to vertex $j$includes all vertices from vertex $0$to vertex $N-1$, let $f(i,j)=N$.
</li>

</ul>

</li>

</ul>

<p>
Note that the path from vertex $i$to vertex $j$in tree $T$includes vertices $i$and $j$.
</p>

<p>
Find the value of $\displaystyle \sum_{0\le i \le j < N} f(i,j)$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\le N\le 2\times 10^5$
</li>

<li>
$0\le u_i < v_i < N$
</li>

<li>
The graph given in the input is a tree.
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

$N$$u_1$$v_1$$u_2$$v_2$$\vdots$$u_{N-1}$$v_{N-1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the value of $\displaystyle \sum_{0\le i \le j < N} f(i,j)$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2
0 1

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
We have $f(0,0)=1,f(0,1)=2,f(1,1)=0$. Thus, output $1+2+0=3$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
0 1
0 2
2 3
2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

16

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

7
1 4
2 6
0 5
0 3
2 5
1 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

16

</div>

</section>

</div>

</span>

</span>

</div>
