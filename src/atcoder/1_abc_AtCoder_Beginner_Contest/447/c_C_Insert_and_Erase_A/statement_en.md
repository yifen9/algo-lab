
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
You are given strings $S$and $T$consisting of uppercase English letters.
</p>

<p>
You may perform the following two types of operations any number of times (possibly zero) in any order:
</p>

<ul>

<li>
Insert one character `A`at any position in $S$(possibly the beginning or the end).
</li>

<li>
Choose one character `A`in $S$and delete it. The remaining characters are concatenated in their original order.
</li>

</ul>

<p>
Determine whether it is possible to make $S$equal to $T$, and if so, find the minimum total number of operations required.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$S$and $T$are strings of uppercase English letters with length between $1$and $3\times 10^5$, inclusive.
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

$S$$T$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If it is possible to make $S$equal to $T$, output the minimum total number of operations required; otherwise, output `-1`.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

ABC
BACA

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
It is possible to make $S$equal to $T$in three operations in total, as follows:
</p>

<ul>

<li>
Insert one `A`between the second and third characters of $S$. Now, $S=$`ABAC`.
</li>

<li>
Delete the first character of $S$, which is `A`. Now, $S=$`BAC`.
</li>

<li>
Insert one `A`at the end of $S$. Now, $S=$`BACA`.
</li>

</ul>

<p>
It is impossible to make $S$equal to $T$in two or fewer operations, so the answer is $3$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

ABC
ARC

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1

</div>

<p>
No matter how operations are performed, it is impossible to make $S$equal to $T$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

ABC
ABC

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

0

</div>

<p>
No operations need to be performed.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

AAAWAZAAAABAAAU
AWAAZABAAAAAUA

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

9

</div>

</section>

</div>

</span>

</span>

</div>
