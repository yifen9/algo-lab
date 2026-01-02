
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
There are $N$Christmas trees on a two-dimensional plane. The $i$-th $(1\le i\le N)$Christmas tree is located at coordinates $(X_i,Y_i)$.
</p>

<p>
You are given $Q$queries. Process the queries in order. Each query is one of the following:
</p>

<ul>

<li>
Type $1$: Given in the form `1 i x y`. Change the coordinates of the $i$-th Christmas tree to $(x,y)$.
</li>

<li>
Type $2$: Given in the form `2 L R x y`. Output the Manhattan distance from the coordinates $(x,y)$to the farthest Christmas tree among the $L,L+1,\ldots,R$-th Christmas trees.
</li>

</ul>

<p>
Here, the Manhattan distance between coordinates $(x_1,y_1)$and coordinates $(x_2,y_2)$is defined as $|x_1-x_2|+|y_1-y_2|$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N,Q\le 2\times 10^5$
</li>

<li>
$-10^9\le X_i,Y_i\le 10^9$
</li>

<li>
$1\le i\le N$
</li>

<li>
$1\le L\le R\le N$
</li>

<li>
$-10^9\le x,y\le 10^9$
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

$N$$Q$$X_1$$Y_1$$X_2$$Y_2$$\vdots$$X_N$$Y_N$$\text{query}_1$$\text{query}_2$$\vdots$$\text{query}_Q$
</div>

<p>
Here, the $i$-th query $\text{query}_i$is given in one of the following formats:
</p>

<div>

$1$$i$$x$$y$
</div>

<div>

$2$$L$$R$$x$$y$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers to the queries, separated by newlines, according to the instructions in the problem statement.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 4
-1 -1
1 2
-2 1
2 1 2 0 0
2 1 3 -1 2
1 1 0 1
2 1 3 -1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
3
2

</div>

<p>
Initially, the $1$st, $2$nd, $3$rd Christmas trees are located at coordinates $(-1,-1)$, $(1,2)$, $(-2,1)$, respectively.
</p>

<p>
Each query is processed as follows:
</p>

<ul>

<li>
The Manhattan distances from the $1$st and $2$nd Christmas trees to coordinates $(0,0)$are $2$and $3$, respectively. Thus, output $3$, which is the maximum value among $2,3$.
</li>

<li>
The Manhattan distances from the $1$st, $2$nd, $3$rd Christmas trees to coordinates $(-1,2)$are $3$, $2$, $2$, respectively. Thus, output $3$, which is the maximum value among $3,2,2$.
</li>

<li>
Change the coordinates of the $1$st Christmas tree to $(0,1)$. The coordinates of the $1$st, $2$nd, $3$rd Christmas trees become $(0,1),(1,2),(-2,1)$, respectively.
</li>

<li>
The Manhattan distances from the $1$st, $2$nd, $3$rd Christmas trees to coordinates $(-1,2)$are $2$, $2$, $2$, respectively. Thus, output $2$, which is the maximum value among $2,2,2$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 7
-9 5
-2 -9
10 -6
9 8
2 9
1 3 -9 -6
2 3 4 2 7
1 4 -2 -10
2 1 2 0 -10
2 3 4 10 -9
2 3 4 8 7
2 5 5 0 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

24
24
22
30
9

</div>

</section>

</div>

</span>

</span>

</div>
