
<div>

<span>

<span>

<p>
Score : $900$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a prime number $p$and an $N \times N$matrix $A = (A_{i,j})$($1\leq i,j\leq N$). Each element of $A$is an integer between $0$and $p-1$, inclusive.
</p>

<p>
Consider a matrix $B$obtained by replacing each zero in $A$with an integer between $1$and $p-1$, inclusive. There are $(p-1)^K$such matrices $B$, where $K$is the number of zeros in $A$.
</p>

<p>
Find each element, modulo $p$, of the sum of $B^p$over all possible $B$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 100$
</li>

<li>
$p$is a prime such that $1 \leq p \leq 10^9$.
</li>

<li>
$0 \leq A_{i,j} \leq p-1$
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

$N$$p$$A_{1,1}$$\cdots$$A_{1,N}$$\vdots$$A_{N,1}$$\cdots$$A_{N,N}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $N$lines.
</p>

<p>
The $i$-th line should contain, in the order $j=1,\ldots,N$, the $(i,j)$element of the sum, modulo $p$, of $B^p$over all possible $B$, separated by spaces.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2 3
0 1
0 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

0 2
1 2

</div>

<p>
$B^p$for all possible $B$are as follows:
</p>

<ul>

<li>
$\begin{pmatrix}1&1 \\ 1&2\end{pmatrix}^3=\begin{pmatrix}5&8 \\ 8&13\end{pmatrix}$
</li>

<li>
$\begin{pmatrix}1&1 \\ 2&2\end{pmatrix}^3=\begin{pmatrix}9&9 \\ 18&18\end{pmatrix}$
</li>

<li>
$\begin{pmatrix}2&1 \\ 1&2\end{pmatrix}^3=\begin{pmatrix}14&13 \\ 13&14\end{pmatrix}$
</li>

<li>
$\begin{pmatrix}2&1 \\ 2&2\end{pmatrix}^3=\begin{pmatrix}20&14 \\ 28&20\end{pmatrix}$
</li>

</ul>

<p>
Print each element, modulo $p=3$, of their sum $\begin{pmatrix}48&44 \\ 67&65\end{pmatrix}$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 2
1 0 0
0 1 0
0 0 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1 1 1
1 1 1
1 1 1

</div>

<p>
$B^p$for all possible $B$are as follows:
</p>

<ul>

<li>
$\begin{pmatrix}1&1&1 \\ 1&1&1 \\ 1&1&1\end{pmatrix}^2=\begin{pmatrix}3&3&3\\3&3&3\\3&3&3\end{pmatrix}$
</li>

</ul>

<p>
Print each element, modulo $p=2$, of their sum $\begin{pmatrix}3&3&3\\3&3&3\\3&3&3\end{pmatrix}$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

4 13
0 1 2 0
3 4 0 5
0 6 0 7
8 9 0 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

8 0 6 5
11 1 8 5
8 0 4 12
8 0 1 9

</div>

</section>

</div>

</span>

</span>

</div>
