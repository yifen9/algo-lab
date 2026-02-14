
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
There are $N$cells, cell $1,$cell $2,\ldots,$cell $N$, arranged in a line.
Cell $i$has an integer $A_i\ (i \le A_i \le N)$written on it.
</p>

<p>
For each of $s=1,2,\ldots,N$, solve the following problem.
</p>

<ul>

<li>
Initially, place a piece on cell $s$. After performing the operation "let $x$be the integer written on the cell where the piece is placed, and then move the piece to cell $x$" $10^{100}$times, output the number of the cell where the piece is placed.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N \le 5\times10^5$
</li>

<li>
$i \le A_i \le N\ (1 \le i \le N)$
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

$N$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for $s=1,2,\ldots,N$in this order on a single line, separated by spaces.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

7
2 4 7 5 5 6 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

5 5 7 5 5 6 7

</div>

<p>
For $s=1$, the piece moves as shown in the following figure.
</p>

<p>

<img src="https://img.atcoder.jp/abc445/c54c58fe4877e457dc58520027e2700f.png">

</img>

</p>

<p>
When the piece is placed on cell $5$, the operation does not move the piece, so the answer for $s=1$is $5$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
1 2 3 4 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1 2 3 4 5

</div>

<p>
It is possible that the piece never moves.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

15
11 3 10 7 15 10 10 11 11 13 11 12 14 14 15

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

11 14 14 14 15 14 14 11 11 14 11 12 14 14 15

</div>

</section>

</div>

</span>

</span>

</div>
