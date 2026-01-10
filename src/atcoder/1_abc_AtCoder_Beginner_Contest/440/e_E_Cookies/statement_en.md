
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $10^{100}$cookies of each of $N$types. The deliciousness per cookie of the $i$-th type is $A_i$.
</p>

<p>
You will choose a total of $K$cookies from these. Two ways of choosing cookies are considered the same if and only if the multisets of types of chosen cookies match.
</p>

<p>
For each of the $\binom{N+K-1}{K}$ways of choosing, consider the sum of deliciousness of the chosen cookies. Let $S_1,S_2,\dots$be these sums in descending order, with duplicates included. Find $S_1,\dots,S_X$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N \leq 50$
</li>

<li>
$1 \leq K \leq 10^5$
</li>

<li>
$1 \leq X \leq \min\left(10^5, \binom{N+K-1}{K}\right)$
</li>

<li>
$-10^9 \leq A_i \leq 10^9$
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

$N$$K$$X$$A_1$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $S_1,S_2,\dots$be the possible sums of deliciousness of the chosen $K$cookies in descending order, with duplicates included. Output $S_1,\dots,S_X$in this order, separated by newlines.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2 4 3
20 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

80
70
60

</div>

<p>
There are $5$ways to choose $4$cookies: "$k$cookies of type $1$and $4-k$cookies of type $2$" $(0\leq k \leq 4)$, where the sums of deliciousness of the chosen cookies are $80,70,60,50,40$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 100000 5
-1 -1 -1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-100000
-100000
-100000
-100000
-100000

</div>

<p>
Different ways of choosing cookies may result in the same sum of deliciousness.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

9 14142 13
31 41 59 26 53 58 97 93 23

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

1371774
1371770
1371766
1371762
1371758
1371754
1371750
1371746
1371742
1371738
1371736
1371735
1371734

</div>

</section>

</div>

</span>

</span>

</div>
