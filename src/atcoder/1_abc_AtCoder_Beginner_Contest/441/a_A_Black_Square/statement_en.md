
<div>

<span>

<span>

<p>
Score : $100$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a grid with $10^{100}$rows and $10^{100}$columns.

In what follows, the cell at the $i$-th row from the top and $j$-th column from the left is denoted as cell $(i,j)$.
</p>

<p>
In this grid, only the $100\times 100$region with cell $(P,Q)$as the top-left cell is painted black, and all other cells are painted white.

Determine whether cell $(X,Y)$is painted black.  
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq P,Q,X,Y \leq 10000$
</li>

<li>
$P,Q,X,Y$are integers.
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

$P$$Q$$X$$Y$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If cell $(X,Y)$is painted black, print `Yes`; otherwise, print `No`.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 3
5 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes

</div>

<p>
The $100\times 100$region with cell $(3,3)$as the top-left cell is painted black.

Cell $(5,10)$is included in this region, so print `Yes`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 5
10 1000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No

</div>

<p>
The $100\times 100$region with cell $(5,5)$as the top-left cell is painted black.

Cell $(10,1000)$is not included in this region, so print `No`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

1 2
1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

No

</div>

<p>
The $100\times 100$region with cell $(1,2)$as the top-left cell is painted black.

Cell $(1,1)$is not included in this region, so print `No`.
</p>

</section>

</div>

</span>

</span>

</div>
