
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$researchers, numbered $1, 2, \ldots, N$.
</p>

<p>
There are $M$conflicts of interest among the researchers; for $i = 1, 2, \ldots, M$, researchers $A_i$and $B_i$have a conflict of interest with each other.
</p>

<p>
The reviewers of a paper must be three distinct researchers who are different from the author of the paper and have no conflict of interest with the author.
</p>

<p>
For $i = 1, 2, \ldots, N$, solve the following problem:
</p>

<ul>

<li>
Find the number of possible triples of reviewers for a paper authored by researcher $i$.
</li>

</ul>

<p>
Assume that all papers are single-authored.
</p>

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
$0 \leq M \leq 2 \times 10^5$
</li>

<li>
$1 \leq A_i, B_i \leq N$
</li>

<li>
$A_i \neq B_i$
</li>

<li>
$(A_i, B_i) \neq (A_j, B_j)$if $i \neq j$.
</li>

<li>
$(A_i, B_i) \neq (B_j, A_j)$if $i \neq j$.
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

$N$$M$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_M$$B_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answers for $i = 1, 2, \ldots, N$in this order, separated by spaces.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

6 5
1 2
1 4
2 3
5 3
3 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

0 1 0 4 4 10

</div>

<p>
Below, we represent a set of researchers by the set of their numbers.
</p>

<ul>

<li>

<p>
There are no possible triples of reviewers for a paper authored by researcher $1$.
</p>

</li>

<li>

<p>
The possible triple of reviewers for a paper authored by researcher $2$is $\lbrace 4, 5, 6 \rbrace$, which is $1$triple.
</p>

</li>

<li>

<p>
There are no possible triples of reviewers for a paper authored by researcher $3$.
</p>

</li>

<li>

<p>
The possible triples of reviewers for a paper authored by researcher $4$are $\lbrace 2, 3, 5 \rbrace, \lbrace 2, 3, 6 \rbrace, \lbrace 2, 5, 6 \rbrace, \lbrace 3, 5, 6 \rbrace$, which is $4$triples.
</p>

</li>

<li>

<p>
The possible triples of reviewers for a paper authored by researcher $5$are $\lbrace 1, 2, 4 \rbrace, \lbrace 1, 2, 6 \rbrace, \lbrace 1, 4, 6 \rbrace, \lbrace 2, 4, 6 \rbrace$, which is $4$triples.
</p>

</li>

<li>

<p>
The possible triples of reviewers for a paper authored by researcher $6$are $\lbrace 1, 2, 3 \rbrace, \lbrace 1, 2, 4 \rbrace, \lbrace 1, 2, 5 \rbrace, \lbrace 1, 3, 4 \rbrace, \lbrace 1, 3, 5 \rbrace, \lbrace 1, 4, 5 \rbrace, \lbrace 2, 3, 4 \rbrace, \lbrace 2, 3, 5 \rbrace, \lbrace 2, 4, 5 \rbrace, \lbrace 3, 4, 5 \rbrace$, which is $10$triples.
</p>

</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

7 3
1 2
3 4
5 6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

10 10 10 10 10 10 20

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

6 9
3 6
2 5
2 3
4 3
1 5
6 2
3 1
5 3
2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

1 0 0 1 0 1

</div>

</section>

</div>

</span>

</span>

</div>
