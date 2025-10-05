
<div>

<span>

<span>

<p>
Score : $800$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Snuke the wizard has $N$magical lamps numbered $1$to $N$.
The cost of the $i$-th lamp is $a_i$.
Initially, none of the lamps are lit.
</p>

<p>
Snuke has an integer value called MP, which is initially $X$.
When Snuke lights a lamp with cost $x$, his MP decreases by $x$.
Each time Snuke lights one lamp, the cost of all lamps with cost at least $1$decreases by $1$.
</p>

<p>
There are $N!$possible orders to light the lamps. Find the number, modulo $998244353$, of such orders where MP never becomes negative.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N \le 100$
</li>

<li>
$0 \le a_i \le 10^{9}$
</li>

<li>
$0 \le X \le 10^9$
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

$N$$X$$a_1$$a_2$$\dots$$a_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 1
0 1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3

</div>

<p>
We explain one order where MP never becomes negative.
</p>

<ul>

<li>
First, light lamp $1$. MP decreases by $0$.
</li>

<li>
Next, light lamp $3$. MP decreases by $1$.
</li>

<li>
Finally, light lamp $2$. MP decreases by $0$.
</li>

</ul>

<p>
Note that the cost of a lamp never becomes negative.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6 8
2 1 4 8 1 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

176

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

20 50
0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

63942667

</div>

<p>
Do not forget to find the remainder modulo $998244353$.
</p>

</section>

</div>

</span>

</span>

</div>
