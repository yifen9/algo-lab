
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
You are given integers $N$and $M$, a digit string $S$of length $N$, and a digit string $T$of length $M$. Here, a digit string is a string consisting of digits from `0`to `9`.
</p>

<p>
You can perform the following operation zero or more times:
</p>

<ul>

<li>
Choose one character from $T$and increase the chosen digit by $1$. However, if the chosen digit is `9`, change it to `0`.
</li>

</ul>

<p>
Find the minimum number of operations required to make $T$a substring (
<strong>
contiguous
</strong>
subsequence) of $S$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le M\le N\le 100$
</li>

<li>
$N$and $M$are integers.
</li>

<li>
$S$is a digit string of length $N$.
</li>

<li>
$T$is a digit string of length $M$.
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

$N$$M$$S$$T$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the minimum number of operations required to make $T$a substring of $S$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 2
2025
91

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
You can make $T$a substring of $S$with two operations as follows:
</p>

<ul>

<li>
Perform the operation on the $2$nd character of $T$. $T=$`91`becomes $T=$`92`.
</li>

<li>
Perform the operation on the $1$st character of $T$. $T=$`92`becomes $T=$`02`.
</li>

</ul>

<p>
`02`is a substring from the $2$nd character to the $3$rd character of $S$.
</p>

<p>
It is impossible to make $T$a substring of $S$with less than two operations, so output $2$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 2
438
38

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

<p>
`38`is a substring of `438`from the beginning. Thus, output $0$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5 5
00000
11111

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

45

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

8 3
20251227
438

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

13

</div>

</section>

</div>

</span>

</span>

</div>
