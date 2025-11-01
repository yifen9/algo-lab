
<div>

<span>

<span>

<p>
Score : $625$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$sets $S_1, \ldots,S_N$. Initially, all sets are empty.
</p>

<p>
You are given $Q$queries in the following formats. Process them in order.
</p>

<ul>

<li>
Type $1$: Given as `1 L R x`. For each $S_i$satisfying $L \leq i \leq R$, add $x$.
</li>

<li>
Type $2$: Given as `2 L R x`. For each $S_i$satisfying $L \leq i \leq R$, remove $x$.
</li>

<li>
Type $3$: Given as `3 L R`. Find the maximum number of elements among $S_i$satisfying $L \leq i \leq R$, and the number of sets that achieve this maximum.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N \leq 3\times 10^5$
</li>

<li>
$1\leq Q \leq 3\times 10^5$
</li>

<li>
For each query, $1 \leq L \leq R \leq N$.
</li>

<li>
For type $1,2$queries, $1 \leq x \leq 60$.
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

$N$$Q$$\mathrm{query}_1$$\vdots$$\mathrm{query}_Q$
</div>

<p>
Here, $\mathrm{query}_i$represents the $i$-th query, and each is given in one of the following formats as shown in the problem statement:
</p>

<div>

$1$$L$$R$$x$
</div>

<div>

$2$$L$$R$$x$
</div>

<div>

$3$$L$$R$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $q$be the number of type $3$queries, and print $q$lines.

The $i$-th line should contain $x,y$separated by a space, where $x$is the maximum number of elements and $y$is the number of sets that achieve this maximum for the $i$-th type $3$query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 7
1 1 2 10
1 2 4 20
3 1 3
2 1 2 20
1 2 3 10
3 1 2
3 1 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2 1
1 2
2 1

</div>

<ul>

<li>
Initially $(S_1,S_2,S_3,S_4)=(\lbrace\rbrace,\lbrace\rbrace,\lbrace\rbrace,\lbrace\rbrace)$.
</li>

<li>
The $1$-st query adds $10$to $S_1,S_2$, resulting in $(S_1,S_2,S_3,S_4)=(\lbrace 10\rbrace,\lbrace 10\rbrace,\lbrace\rbrace,\lbrace\rbrace)$.
</li>

<li>
The $2$-nd query adds $20$to $S_2,S_3,S_4$, resulting in $(S_1,S_2,S_3,S_4)=(\lbrace 10\rbrace,\lbrace 10,20\rbrace,\lbrace 20\rbrace,\lbrace 20\rbrace)$.
</li>

<li>
For the $3$-rd query, the maximum number of elements among $S_1,S_2,S_3$is $2$achieved by $S_2$, so print `2 1`.
</li>

<li>
The $4$-th query removes $20$from $S_1,S_2$, resulting in $(S_1,S_2,S_3,S_4)=(\lbrace 10\rbrace,\lbrace 10\rbrace,\lbrace 20\rbrace,\lbrace 20\rbrace)$.
</li>

<li>
The $5$-th query adds $10$to $S_2,S_3$, resulting in $(S_1,S_2,S_3,S_4)=(\lbrace 10\rbrace,\lbrace 10\rbrace,\lbrace 10,20\rbrace,\lbrace 20\rbrace)$.
</li>

<li>
For the $6$-th query, the maximum number of elements among $S_1,S_2$is $1$achieved by $S_1,S_2$, so print `1 2`.
</li>

<li>
For the $7$-th query, the maximum number of elements among $S_1,S_2,S_3,S_4$is $2$achieved by $S_3$, so print `2 1`.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
