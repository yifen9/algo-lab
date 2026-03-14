
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
There is a rectangular chocolate consisting of $H$rows and $W$columns of blocks.
</p>

<p>
You are given $Q$queries; process them in order and find the answer to each query. Each query is in one of the following formats:
</p>

<ul>

<li>

<p>
Type $1$: An integer $R$is given. Find the number of chocolate blocks in the bottom $R$rows, then eat them.
</p>

</li>

<li>

<p>
Type $2$: An integer $C$is given. Find the number of chocolate blocks in the rightmost $C$columns, then eat them.
</p>

</li>

</ul>

<p>
When the queries are processed in order, the chocolate remains rectangular after each query is processed, and it has at least $R + 1$rows immediately before processing a type $1$query and has at least $C + 1$columns immediately before processing a type $2$query.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq H, W \leq 100$
</li>

<li>
$1 \leq Q \leq 100$
</li>

<li>
For type $1$queries, $1 \leq R$.
</li>

<li>
When the queries are processed in order, the chocolate has at least $R + 1$rows immediately before processing a type $1$query.
</li>

<li>
For type $2$queries, $1 \leq C$.
</li>

<li>
When the queries are processed in order, the chocolate has at least $C + 1$columns immediately before processing a type $2$query.
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

$H$$W$$Q$$\text{query}_1$$\text{query}_2$$\vdots$$\text{query}_Q$
</div>

<p>
Here, $\text{query}_i$is the $i$-th query, given in one of the following formats:
</p>

<div>

$1$$R$
</div>

<div>

$2$$C$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.
The $i$-th line $(1 \leq i \leq Q)$should contain the answer to the $i$-th query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

7 9 5
2 4
1 3
2 1
2 1
1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

28
15
4
4
9

</div>

<p>
Initially, the chocolate is a rectangle with $7$rows and $9$columns.
</p>

<p>
For the first query, the number of chocolate blocks in the rightmost $4$columns is $28$, so output $28$. The chocolate becomes $7$rows and $5$columns.
</p>

<p>
For the second query, the number of chocolate blocks in the bottom $3$rows is $15$, so output $15$. The chocolate becomes $4$rows and $5$columns.
</p>

<p>
For the third query, the number of chocolate blocks in the rightmost $1$column is $4$, so output $4$. The chocolate becomes $4$rows and $4$columns.
</p>

<p>
For the fourth query, the number of chocolate blocks in the rightmost $1$column is $4$, so output $4$. The chocolate becomes $4$rows and $3$columns.
</p>

<p>
For the fifth query, the number of chocolate blocks in the bottom $3$rows is $9$, so output $9$. The chocolate becomes $1$row and $3$columns.
</p>

</section>

</div>

</span>

</span>

</div>
