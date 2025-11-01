
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<p>
In AtCoder Country, there is a rule that "a truck driver must take a break of at least $B$minutes when driving for $A$minutes or more."
</p>

</blockquote>

<p>
You are given a string $S$of length $N$consisting of `a`and `b`, and positive integers $A$and $B$. Find the number of integer pairs $(l,r)$that satisfy all of the following conditions.
</p>

<ul>

<li>
$1\leq l \leq r \leq N$
</li>

<li>
The number of `a`in the substring from the $l$-th character through the $r$-th character of $S$is greater than or equal to $A$.
</li>

<li>
The number of `b`in the substring from the $l$-th character through the $r$-th character of $S$is less than $B$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N \leq 3\times 10^5$
</li>

<li>
$1 \leq A,B \leq N$
</li>

<li>
$S$is a string of length $N$consisting of `a`and `b`.
</li>

<li>
All input numbers are integers.
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

$N$$A$$B$$S$
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

11 4 2
abbaaabaaba

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
The pairs $(l,r)$that satisfy the conditions are $(4,8),(4,9),(5,9)$, which is three pairs.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

13 1 2
bbbbbbbbbbbbb

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
There are no pairs $(l,r)$that satisfy the conditions.
</p>

</section>

</div>

</span>

</span>

</div>
