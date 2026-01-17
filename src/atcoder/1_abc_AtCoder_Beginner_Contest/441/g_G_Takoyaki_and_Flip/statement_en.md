
<div>

<span>

<span>

<p>
Score : $575$points
</p>

<div>

<section>

### **Problem Statement**

<p>
$N$plates are arranged in a straight line from left to right.
Let us call the $i$-th plate from the left $(1\le i\le N)$plate $i$.
Initially, all plates are placed face-up, and no plates have takoyaki (octopus dumplings) on them.
</p>

<p>
Process a total of $Q$queries of the following three types:
</p>

<ul>

<li>
Type $1$: You are given integers $L,R,X$. For $i=L,L+1,\ldots,R$, if plate $i$is placed face-up, place $X$takoyaki on plate $i$.
</li>

<li>
Type $2$: You are given integers $L,R$. For $i=L,L+1,\ldots,R$, if there is at least one takoyaki on plate $i$, eat all the takoyaki on plate $i$. Flip plate $i$(if the plate is placed face-up, place it face-down; otherwise, place it face-up).
</li>

<li>
Type $3$: You are given integers $L,R$. Print the maximum number of takoyaki on one plate among plates $L,$$L+1,\ldots,$$R$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le2\times10 ^ 5$
</li>

<li>
$1\le Q\le2\times10 ^ 5$
</li>

<li>
In all queries, $1\le L\le R\le N$.
</li>

<li>
In type $1$queries, $1\le X\le10 ^ 9$.
</li>

<li>
There is at least one type $3$query.
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

$N$$Q$$\mathrm{query} _ 1$$\mathrm{query} _ 2$$\vdots$$\mathrm{query} _ Q$
</div>

<p>
Here, $\mathrm{query} _ i$represents the $i$-th $(1\le i\le Q)$query and is given in one of the following formats:
</p>

<div>

$t$$L$$R$$X$
</div>

<div>

$t$$L$$R$
</div>

<p>
These indicate that the $i$-th query is of type $t$and the given integers are $L,R,X$or $L,R$.
Type $1$queries are given in the former format, and other queries are given in the latter format.
</p>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $q$be the number of type $3$queries. Print $q$lines.
The $i$-th line $(1\le i\le q)$should contain the answer to the $i$-th type $3$query from the beginning.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

6 6
1 3 5 4
3 2 3
1 1 6 2
2 3 4
3 1 6
3 2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4
6
2

</div>

<p>
At the time of each query, the state of each plate and the number of takoyaki on it are as shown in the figure below.
</p>

<p>

<img src="https://img.atcoder.jp/abc441/5a1f8a0f9bdb43a16c4f458213f3b8e7.png">

</img>

</p>

<p>
At the time of the second query, among plates $2$and $3$, the one with more takoyaki is plate $3$.
Thus, print `4`, the number of takoyaki on plate $3$, on the first line.
</p>

<p>
At the time of the fifth query, among plates $1,$$2,\ldots,$$6$, the one with the most takoyaki is plate $5$.
Thus, print `6`, the number of takoyaki on plate $5$, on the second line.
</p>

<p>
At the time of the sixth query, among plates $2$and $3$, the one with more takoyaki is plate $2$.
Thus, print `2`, the number of takoyaki on plate $2$, on the third line.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2 8
1 1 2 1000000000
1 1 2 1000000000
2 2 2
1 1 2 1000000000
1 1 2 1000000000
1 1 2 1000000000
3 2 2
3 1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0
5000000000

</div>

<p>
Note that no takoyaki is placed on plates that are placed face-down.
</p>

<p>
Also, note that the answer may be $2 ^ {32}$or more.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

24 30
1 11 24 4326
1 4 16 1149
1 14 20 2331
1 12 14 8930
1 22 23 6989
3 15 20
3 10 19
1 3 12 7988
1 18 23 8450
3 9 19
3 13 15
2 8 15
2 9 14
1 11 17 4062
1 6 15 1721
3 7 13
1 11 20 8541
1 8 10 3748
1 1 17 3252
2 9 23
2 1 23
3 2 22
1 5 23 7468
3 1 12
3 12 19
2 6 24
3 2 14
3 1 15
2 15 19
3 2 14

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

7806
16736
22393
16736
10858
0
7468
7468
0
0
0

</div>

</section>

</div>

</span>

</span>

</div>
