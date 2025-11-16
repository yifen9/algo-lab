
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence $A=(A_1,A_2,\ldots,A_N)$of length $N$and an integer sequence $B=(B_1,B_2,\ldots,B_M)$of length $M$. Here, $N$is 
<strong>
even
</strong>
.
</p>

<p>
You are given $Q$queries. The $q$-th query is given as a triple of integers $(t_q,i_q,x_q)$, and it does the following.
</p>

<ul>

<li>
If $t_q=1$: In this case, $1\leq i_q\leq N$. This query changes $A_{i_q}$to $x_q$.
</li>

<li>
If $t_q=2$: In this case, $1\leq i_q\leq M$. This query changes $B_{i_q}$to $x_q$.
</li>

</ul>

<p>
After processing each query, find the answer to the following subproblem.
</p>

<blockquote>

<p>
Initialize a multiset $X$with $X=\lbrace A_1,A_2,\ldots,A_N\rbrace$.
For $j=1,2,\ldots,M$, perform the following operation:
</p>

<ul>

<li>
Insert $B_j$into $X$. Then, remove one median of $X$from $X$.
</li>

</ul>

<p>
Find the sum of elements in $X$when all operations are finished.
</p>

</blockquote>

<details>

<summary>
What is a median?
</summary>

<p>
When $N$is even, the median of a multiset $X$with $N+1$elements is the $\left(1+\frac{N}{2}\right)$-th value in ascending order among the elements of $X$.

</p>

<p>
For example, the median of $X=\lbrace 1, 3, 4, 5, 8\rbrace$is $4$, and the median of $X=\lbrace 2,2,2\rbrace$is $2$.

</p>

<p>
Note that in this problem, the multiset for which we consider the median always has an odd number of elements.

</p>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N,M,Q\leq 2\times 10^5$
</li>

<li>
$N$is even.
</li>

<li>
$1\leq A_i\leq 10^9$
</li>

<li>
$1\leq B_i\leq 10^9$
</li>

<li>
$t_q\in\lbrace 1,2\rbrace$
</li>

<li>
If $t_q=1$, then $1\leq i_q\leq N$
</li>

<li>
If $t_q=2$, then $1\leq i_q\leq M$
</li>

<li>
$1\leq x_q\leq 10^9$
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

$N$$M$$Q$$A_1$$A_2$$\cdots$$A_N$$B_1$$B_2$$\cdots$$B_M$$t_1$$i_1$$x_1$$\vdots$$t_Q$$i_Q$$x_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $q$-th line should contain the answer to the subproblem immediately after processing the $q$-th query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 2 2
5 1 4 3
1 2
1 3 3
2 1 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

10
13

</div>

<p>
First, the $1$-st query makes $A=(5,1,3,3)$and $B=(1,2)$. In this case, the operations in the subproblem proceed as follows.
</p>

<ul>

<li>
Initialize $X=\lbrace 5,1,3,3\rbrace=\lbrace 1,3,3,5\rbrace$.
</li>

<li>
Insert $B_1=1$into $X$, making $X=\lbrace 1,1,3,3,5\rbrace$. Then, remove one median from $X$, making $X=\lbrace 1,1,3,5\rbrace$.
</li>

<li>
Insert $B_2=2$into $X$, making $X=\lbrace 1,1,2,3,5\rbrace$. Then, remove one median from $X$, making $X=\lbrace 1,1,3,5\rbrace$.
</li>

</ul>

<p>
The sum of elements in $X$when all operations are finished is $1+1+3+5=10$.
</p>

<p>
Next, the $2$-nd query makes $A=(5,1,3,3)$and $B=(5,2)$. In this case, the operations in the subproblem proceed as follows.
</p>

<ul>

<li>
Initialize $X=\lbrace 5,1,3,3\rbrace=\lbrace 1,3,3,5\rbrace$.
</li>

<li>
Insert $B_1=5$into $X$, making $X=\lbrace 1,3,3,5,5\rbrace$. Then, remove one median from $X$, making $X=\lbrace 1,3,5,5\rbrace$.
</li>

<li>
Insert $B_2=2$into $X$, making $X=\lbrace 1,2,3,5,5\rbrace$. Then, remove one median from $X$, making $X=\lbrace 1,2,5,5\rbrace$.
</li>

</ul>

<p>
The sum of elements in $X$when all operations are finished is $1+2+5+5=13$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6 7 5
7 1 2 5 5 3
4 2 5 1 3 3 8
2 1 3
2 7 1
1 3 6
2 4 2
1 5 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

24
20
21
22
21

</div>

</section>

</div>

</span>

</span>

</div>
