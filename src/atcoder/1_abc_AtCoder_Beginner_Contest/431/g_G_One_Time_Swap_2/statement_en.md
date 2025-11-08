
<div>

<span>

<span>

<p>
Score : ${575}$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence $A=(A_1,A_2,\ldots,A_N)$of length $N$.
</p>

<p>
For a pair of integers $(l, r) \ (1\leq l\lt r\leq N)$, let $f(l,r)$be the integer sequence obtained by swapping the $l$-th element and the $r$-th element of $A$.
</p>

<p>
Generate a sequence of integer sequences $B=(B_1,B_2,\ldots,B_{\frac{N(N-1)}{2}})$of length $\frac{N(N-1)}{2}$by the following procedure:
</p>

<ul>

<li>
Prepare an empty sequence $B=()$.
</li>

<li>
For each pair of integers $(l, r)\ (1\leq l\lt r\leq N)$, add $f(l,r)$to $B$.
</li>

<li>
Sort $B$in lexicographical order of sequences.
</li>

</ul>

<p>
You are given $Q$queries; process them in order. The $i$-th query is as follows:
</p>

<ul>

<li>
Given an integer $k$, find one pair of integers $(l, r) \ (1\leq l\lt r\leq N)$such that $B_k=f(l,r)$and output it.
</li>

</ul>

<details>

<summary>
What is lexicographical order of sequences?
</summary>

<p>
A sequence $S = (S_1,S_2,\ldots,S_{|S|})$is 
<strong>
lexicographically smaller
</strong>
than a sequence $T = (T_1,T_2,\ldots,T_{|T|})$if and only if one of the following two conditions holds.
Here, $|S|$and $|T|$represent the lengths of $S$and $T$, respectively.
</p>

<ol>

<li>
$|S| \lt |T|$and $(S_1,S_2,\ldots,S_{|S|}) = (T_1,T_2,\ldots,T_{|S|})$. 
</li>

<li>
There exists an integer $1 \leq i \leq \min\lbrace |S|, |T| \rbrace$such that both of the following hold:

<ul>

<li>
$(S_1,S_2,\ldots,S_{i-1}) = (T_1,T_2,\ldots,T_{i-1})$
</li>

<li>
$S_i$is smaller than $T_i$(as a number).
</li>

</ul>

</li>

</ol>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\leq N\leq 2\times 10^5$
</li>

<li>
$1\leq Q\leq 2\times 10^5$
</li>

<li>
$1\leq A_i\leq N$
</li>

<li>
$1\leq k\leq \frac{N(N-1)}{2}$
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

$N$$Q$$A_1$$A_2$$\ldots$$A_N$$\mathrm{query}_1$$\mathrm{query}_2$$\vdots$$\mathrm{query}_Q$
</div>

<p>
Each query is given in the following format:
</p>

<div>

$k$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $i$-th line should contain the answer to the $i$-th query in the following format:
</p>

<div>

$l$$r$
</div>

<p>
If there are multiple solutions, any of them will be considered correct.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 3
1 2 1 2
1
3
5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2 3
2 4
1 2

</div>

<p>
$f(1, 2) = (2, 1, 1, 2), f(1, 3) = (1, 2, 1, 2), f(1, 4) = (2, 2, 1, 1), f(2, 3) = (1, 1, 2, 2), f(2, 4) = (1, 2, 1, 2), f(3, 4) = (1, 2, 2, 1)$.
</p>

<p>
The sequence $B$obtained by sorting these six sequences in lexicographical order is $B=((1, 1, 2, 2), (1, 2, 1, 2), (1, 2, 1, 2), (1, 2, 2, 1), (2, 1, 1, 2), (2, 2, 1, 1))$.
</p>

<ul>

<li>
For the $1$-st query, the only $(l,r)$such that $B_1=(1,1,2,2)=f(l,r)$is $(l,r)=(2,3)$.
</li>

<li>
For the $2$-nd query, $(l,r)$such that $B_3=(1,2,1,2)=f(l,r)$are $(l,r)=(1,3),(2,4)$. In this case, either one will be considered correct.
</li>

<li>
For the $3$-rd query, the only $(l,r)$such that $B_5=(2,1,1,2)=f(l,r)$is $(l,r)=(1,2)$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 10
1 1 2 7 6 3 5 7 3 3
21
36
9
17
13
24
7
45
33
1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

6 8
2 4
5 7
9 10
8 9
3 9
5 9
1 8
2 10
4 10

</div>

</section>

</div>

</span>

</span>

</div>
