
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
There are $N$intervals on a number line, numbered from $1$to $N$.
</p>

<p>
The left endpoint of interval $i$is at coordinate $0$, and the right endpoint is at coordinate $W_i$. Here, $W_1 < W_2 < \dots < W_N$.
</p>

<p>
You are given $Q$queries; process them in the order they are given. Each query is one of the following three types:
</p>

<ul>

<li>
Type $1$(`1 v`): Let $l$be the coordinate of the current 
<strong>
left endpoint
</strong>
of interval $v$. Translate each of the intervals numbered $v$or less so that its 
<strong>
left endpoint
</strong>
is at coordinate $l$.
</li>

<li>
Type $2$(`2 v`): Let $r$be the coordinate of the current 
<strong>
right endpoint
</strong>
of interval $v$. Translate each of the intervals numbered $v$or less so that its 
<strong>
right endpoint
</strong>
is at coordinate $r$.
</li>

<li>
Type $3$(`3 x`): Output the current number of intervals that contain coordinate $x+\frac{1}{2}$.
</li>

</ul>

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
$1 \leq Q \leq 2 \times 10^5$
</li>

<li>
$1 \leq W_i \leq 10^9$($1 \leq i \leq N$)
</li>

<li>
$W_1 < W_2 < \dots < W_N$
</li>

<li>
For $v$given in queries of types $1$and $2$, $1 \leq v \leq N$.
</li>

<li>
For $x$given in queries of type $3$, $0 \leq x \leq 10^9$.
</li>

<li>
At least one query of type $3$is given.
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

$N$$W_1$$\dots$$W_N$$Q$$\textrm{query}_1$$\textrm{query}_2$$\vdots$$\textrm{query}_Q$
</div>

<p>
$\textrm{query}_j$represents the $j$-th query. Each query is given in one of the following formats:
</p>

<div>

$1$$v$
</div>

<div>

$2$$v$
</div>

<div>

$3$$x$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $q$be the number of queries of type $3$, output $q$lines. The $j$-th line ($1 \leq j \leq q$) should contain the answer to the $j$-th query of type $3$.
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
2 4 6 10
5
2 3
1 2
3 2
2 4
3 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4
1

</div>

<p>
Initially, the intervals in order of their numbers are $[0, 2], [0, 4], [0, 6], [0, 10]$.
</p>

<ul>

<li>
For the $1$st query, the coordinate of the 
<strong>
right endpoint
</strong>
of interval $3$before the operation is $6$, so the intervals after the operation are $[4, 6], [2, 6], [0, 6], [0, 10]$in order of their numbers.
</li>

<li>
For the $2$nd query, the coordinate of the 
<strong>
left endpoint
</strong>
of interval $2$before the operation is $2$, so the intervals after the operation are $[2, 4], [2, 6], [0, 6], [0, 10]$in order of their numbers.
</li>

<li>
For the $3$rd query, the intervals that contain coordinate $2 + \frac{1}{2}$are intervals $1,2,3,4$, which is four intervals, so output $4$.
</li>

<li>
For the $4$th query, the coordinate of the 
<strong>
right endpoint
</strong>
of interval $4$before the operation is $10$, so the intervals after the operation are $[8, 10], [6, 10], [4, 10], [0, 10]$in order of their numbers.
</li>

<li>
For the $5$th query, the intervals that contain coordinate $1 + \frac{1}{2}$is only interval $4$, which is one interval, so output $1$.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
