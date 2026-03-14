
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
You are given a string $S$of length $N$consisting of lowercase English letters.
</p>

<p>
Find the number of pairs of integers $(i, j)$satisfying all of the following conditions:
</p>

<ul>

<li>
$1 \leq i \leq j \leq N$
</li>

<li>
$S_i = S_j$
</li>

<li>
$L \leq j - i \leq R$
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 5 \times 10^5$
</li>

<li>
$1 \leq L \leq R \leq N - 1$
</li>

<li>
$N, L, R$are integers.
</li>

<li>
$S$is a string of length $N$consisting of lowercase English letters.
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

$N$$L$$R$$S$
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

6 2 4
aabcba

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2

</div>

<p>
The pairs of integers satisfying all the conditions in the problem statement are $(i, j) = (2, 6), (3, 5)$, for a total of two pairs.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

9 3 6
aaaaaaaaa

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

18

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10 2 6
aabbccaabb

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

6

</div>

</section>

</div>

</span>

</span>

</div>
