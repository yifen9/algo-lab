
<div>

<span>

<span>

<p>
Score : $425$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a pond with a circumference of $M$, and on its shore stand one hut and $N$people.

For a real number $x$$(0\leq x <M)$, define point $x$as the location that is $x$distance clockwise from the hut.

The $i$-th person is at point $A_i$.

<strong>
Multiple people may be standing at the same location.
</strong>

</p>

<p>
Additionally, an integer $C$not greater than $N$is given.
For $i=0,1,\ldots,M-1$, define $X_i$as follows:
</p>

<ol>

<li>
Takahashi starts at point $(i+0.5)$and begins moving clockwise.
</li>

<li>
Takahashi continues moving (clockwise) as long as the total number of people he has met is less than $C$, and stops when it becomes $C$or more. Here, "meeting a person at point $y$" means that Takahashi reaches point $y$.
</li>

<li>
Let $X_i$be the number of people Takahashi met before stopping. Here, if there are multiple people at the point where Takahashi stopped, all the people there are counted as people he met, and particularly, $X_i$may be greater than $C$.  
</li>

</ol>

<p>
Find the sum of $X_i$over $i=0,1,\ldots,M-1$, that is, $\displaystyle\sum_{i=0}^{M-1} X_i$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N\leq 5\times 10^5$
</li>

<li>
$1\leq M\leq 10^{12}$
</li>

<li>
$0\leq A_i\leq M-1$
</li>

<li>
$1\leq C\leq N$
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

$N$$M$$C$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the sum of $X_i$over $i=0,1,\ldots,M-1$on a single line.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 3 2
1 2 1 0 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

9

</div>

<p>
When $i=0$, Takahashi starts at point $0.5$and moves clockwise. Then, the following happens:
</p>

<ul>

<li>
At point $1$, he meets the $1$st, $3$rd, and $5$th people, a total of three people, and the total number of people met so far is $3$. This is not less than $C=2$, so Takahashi stops there. Therefore, $X_0=3$.
</li>

</ul>

<p>
When $i=1$, Takahashi starts at point $1.5$and moves clockwise. Then, the following happens:
</p>

<ul>

<li>
At point $2$, he meets the $2$nd person. The total number of people met so far is $1$, so he continues moving.
</li>

<li>
At point $0$, he meets the $4$th person, and the total number of people met so far is $2$. This is not less than $C=2$, so Takahashi stops there. Therefore, $X_1=2$.
</li>

</ul>

<p>
When $i=2$, Takahashi starts at point $2.5$and moves clockwise. Then, the following happens:
</p>

<ul>

<li>
At point $0$, he meets the $4$th person. The total number of people met so far is $1$, so he continues moving.
</li>

<li>
At point $1$, he meets the $1$st, $3$rd, and $5$th people, a total of three people, and the total number of people met so far is $4$. This is not less than $C=2$, so Takahashi stops there. Therefore, $X_2=4$.
</li>

</ul>

<p>
Therefore, the answer is $X_0+X_1+X_2=3+2+4=9$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1 1000000000000 1
1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1000000000000

</div>

<p>
Regardless of the starting position, Takahashi stops when he meets the only person standing around the pond, who is at point $1$.

Therefore, $X_i=1$regardless of $i$, and the answer is $10^{12}$.
</p>

</section>

</div>

</span>

</span>

</div>
