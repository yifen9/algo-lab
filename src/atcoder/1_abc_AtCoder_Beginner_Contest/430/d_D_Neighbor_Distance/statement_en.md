
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a number line, and initially person $0$is standing alone at coordinate $0$.
</p>

<p>
From now on, persons $1,2,\dots,N$will arrive in this order and stand on the number line.

Person $i$stands at coordinate $X_i$. Here, $X_i \ge 1$, and $X_i$is distinct for all persons.
</p>

<p>
Each time a person arrives, answer the following question.
</p>

<ul>

<li>
Suppose that currently $r+1$persons $0,1,\dots,r$are standing on the number line.
</li>

<li>
Here, define $d_i$as the distance to the nearest other person from person $i$.
<ul>

<li>
More formally, $\displaystyle d_i = \min_{0 \le j \le r, j \neq i} \vert X_i - X_j \vert$.
</li>

</ul>

</li>

<li>
Find the sum of this $d$, that is, $\displaystyle \sum_{i=0}^r d_i$.
</li>

</ul>

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
$1 \le N \le 5 \times 10^5$
</li>

<li>
$1 \le X_i \le 10^9$
</li>

<li>
$X_i \neq X_j$if $i \neq j$.
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

$N$$X_1$$X_2$$\dots$$X_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $N$lines.

The $i$-th line ( $1 \le i \le N$) should contain the answer to the question when person $i$arrives.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

10
5 2 7 4 108728325 390529120 597713292 322456626 845148281 812604915

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

10
7
8
8
108728326
390529121
523096670
452057486
699492475
517144218

</div>

<p>
In this input, $10$persons arrive.

The first four persons are explained below.
</p>

<ul>

<li>
When person $1$arrives, there are persons at coordinates $0,5$.
<ul>

<li>
The required value is $5+5=10$.
</li>

</ul>

</li>

<li>
When person $2$arrives, there are persons at coordinates $0,2,5$.
<ul>

<li>
The required value is $2+2+3=7$.
</li>

</ul>

</li>

<li>
When person $3$arrives, there are persons at coordinates $0,2,5,7$.
<ul>

<li>
The required value is $2+2+2+2=8$.
</li>

</ul>

</li>

<li>
When person $4$arrives, there are persons at coordinates $0,2,4,5,7$.
<ul>

<li>
The required value is $2+2+1+1+2=8$.
</li>

</ul>

</li>

</ul>

</section>

</div>

</span>

</span>

</div>
