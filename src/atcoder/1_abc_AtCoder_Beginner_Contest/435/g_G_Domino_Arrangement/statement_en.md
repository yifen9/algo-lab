
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
There are $N$cells numbered from $1$to $N$. Initially, no cell is painted with any color.
</p>

<p>
There are $M$types of colors, and with the $i$-th color, you can paint any number of cells you like among cells $L_i,L_i+1,\ldots,R_i$.
</p>

<p>
Find the number, modulo $998244353$, of ways to paint the cells that satisfy the following condition:
</p>

<ul>

<li>
For every cell $i$, if that cell is painted with a color, then exactly one of cells $i-1$and $i+1$is painted with the same color as cell $i$.
<ul>

<li>
Here, cells $0$and $N+1$are considered to be not painted with any color.
</li>

</ul>

</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N,M \leq 5\times 10^5$
</li>

<li>
$1\leq L_i \leq R_i \leq N$
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

$N$$M$$L_1$$R_1$$\vdots$$L_M$$R_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 2
1 3
1 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

11

</div>

<p>
The first color can paint cells $1,2,3$, and the second color can paint cells $1,2,3,4,5$.
</p>

<p>
There are $11$ways to paint that satisfy the condition, as follows:
</p>

<p>

<img src="https://img.atcoder.jp/abc435/03fd1b0a01e7b5e51ebb60b7b4f1a610.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 3
1 1
2 2
3 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

<p>
The one way of not painting any cell satisfies the condition.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

500000 10
1 499999
2 499998
3 499997
4 499996
5 499995
6 499994
7 499993
8 499992
9 499991
10 499990

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

775503999

</div>

<p>
Find the count modulo $998244353$.
</p>

</section>

</div>

</span>

</span>

</div>
