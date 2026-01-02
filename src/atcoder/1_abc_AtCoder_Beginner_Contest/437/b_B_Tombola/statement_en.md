
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
There is a grid with $H$rows and $W$columns. Each square has one integer written on it, and these integers are distinct. The square at the $i$-th row from the top and $j$-th column from the left has the integer $A_{i,j}$written on it.
</p>

<p>
Now, the host called out $N$distinct integers $B_1, \dots, B_N$.
</p>

<p>
If you find, for each row, how many of the integers called out by the host are contained in that row, what is the maximum value among these?
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq H \leq 3$
</li>

<li>
$1 \leq W \leq 5$
</li>

<li>
$1 \leq N \leq 90$
</li>

<li>
$1 \leq A_{i,j} \leq 90$
</li>

<li>
$A_{i,j}$are distinct.
</li>

<li>
$1 \leq B_i \leq 90$
</li>

<li>
$B_i$are distinct.
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

$H$$W$$N$$A_{1,1}$$\cdots$$A_{1,W}$$\vdots$$A_{H,1}$$\cdots$$A_{H,W}$$B_1$$\vdots$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer in one line.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 4 5
12 3 5 7
6 10 11 9
1 2 4 8
2
4
9
6
11

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3

</div>

<ul>

<li>
Among the integers in the $1$-st row from the top, $0$integers were called out by the host.
</li>

<li>
Among the integers in the $2$-nd row from the top, $3$integers $6,11,9$were called out by the host.
</li>

<li>
Among the integers in the $3$-rd row from the top, $2$integers $2,4$were called out by the host.
</li>

</ul>

<p>
Thus, the answer is the maximum value among $0,3,2$, which is $3$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 5 2
81 63 31 16 15
30 3 6 54 24
26 41 48 64 66
44
79

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

3 5 12
78 19 70 58 83
12 30 80 20 27
48 71 8 43 82
82
30
43
8
80
70
20
78
12
71
19
48

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

5

</div>

</section>

</div>

</span>

</span>

</div>
