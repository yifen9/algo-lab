
<div>

<span>

<span>

<p>
Score : $800$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$rabbits on a number line.
The rabbits are conveniently numbered $1$through $N$.
The coordinate of the initial position of rabbit $i$is $x_i$.
</p>

<p>
The rabbits will now take exercise on the number line, by performing 
<em>
sets
</em>
described below.
A set consists of $M$
<em>
jumps
</em>
. The $j$-th jump of a set is performed by rabbit $a_j$($2≤a_j≤N-1$).
For this jump, either rabbit $a_j-1$or rabbit $a_j+1$is chosen with equal probability (let the chosen rabbit be rabbit $x$), then rabbit $a_j$will jump to the symmetric point of its current position with respect to rabbit $x$.
</p>

<p>
The rabbits will perform $K$sets in succession.
For each rabbit, find the expected value of the coordinate of its eventual position after $K$sets are performed.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3≤N≤10^5$
</li>

<li>
$x_i$is an integer.
</li>

<li>
$|x_i|≤10^9$
</li>

<li>
$1≤M≤10^5$
</li>

<li>
$2≤a_j≤N-1$
</li>

<li>
$1≤K≤10^{18}$
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

$N$$x_1$$x_2$$...$$x_N$$M$$K$$a_1$$a_2$$...$$a_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $N$lines.
The $i$-th line should contain the expected value of the coordinate of the eventual position of rabbit $i$after $K$sets are performed.
The output is considered correct if the absolute or relative error is at most $10^{-9}$.
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
-1 0 2
1 1
2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

-1.0
1.0
2.0

</div>

<p>
Rabbit $2$will perform the jump.
If rabbit $1$is chosen, the coordinate of the destination will be $-2$.
If rabbit $3$is chosen, the coordinate of the destination will be $4$.
Thus, the expected value of the coordinate of the eventual position of rabbit $2$is $0.5×(-2)+0.5×4=1.0$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
1 -1 1
2 2
2 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1.0
-1.0
1.0

</div>

<p>
$x_i$may not be distinct.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5
0 1 3 6 10
3 10
2 3 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

0.0
3.0
7.0
8.0
10.0

</div>

</section>

</div>

</span>

</span>

</div>
