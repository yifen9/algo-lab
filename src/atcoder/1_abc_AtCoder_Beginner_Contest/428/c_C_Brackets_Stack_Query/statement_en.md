
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
A string $T$is called a good bracket sequence if and only if it satisfies the following condition:
</p>

<ul>

<li>

<p>
$T$can be made into an empty string by repeating the following operation zero or more times:
</p>

<ul>

<li>
Choose `()`contained in $T$as a (contiguous) substring and remove it.
</li>

</ul>

</li>

</ul>

<p>
For example, `()`, `(()())`, and the empty string are good bracket sequences, but `)()(`and `)))`are not good bracket sequences.
</p>

<p>
There is a string $S$. Initially, $S$is an empty string.

Process $Q$queries in the order they are given. After each query, determine whether $S$is a good bracket sequence.

There are two types of queries:
</p>

<ul>

<li>
`1 c`: A character $c$is given. $c$is either `(`or `)`. Append $c$to the end of $S$.
</li>

<li>
`2`: Remove the last character of $S$. It is guaranteed that $S$is not an empty string at this time.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq Q \leq 8 \times 10^5$
</li>

<li>
$c$in queries of the first type is `(`or `)`.
</li>

<li>
It is guaranteed that $S$is not empty when a query of the second type is given.
</li>

<li>
$Q$is an integer.
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
The input is given from Standard Input in the following format, where $\mathrm{query}_i$denotes the $i$-th query.
</p>

<div>

$Q$$\mathrm{query}_1$$\mathrm{query}_2$$\vdots$$\mathrm{query}_Q$
</div>

<p>
Each query is given in one of the following two formats:
</p>

<div>

$1$$c$
</div>

<div>

$2$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $i$-th line should contain `Yes`if the string $S$immediately after processing the $i$-th query is a good bracket sequence, and `No`otherwise.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

8
1 (
2
1 (
1 )
2
1 (
1 )
1 )

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

No
Yes
No
Yes
No
No
No
Yes

</div>

<p>
$S$immediately after processing the $1$st query is `(`, which is not a good bracket sequence.

$S$immediately after processing the $2$nd query is an empty string, which is a good bracket sequence.

$S$immediately after processing the $3$rd query is `(`, which is not a good bracket sequence.

$S$immediately after processing the $4$th query is `()`, which is a good bracket sequence.

$S$immediately after processing the $5$th query is `(`, which is not a good bracket sequence.

$S$immediately after processing the $6$th query is `((`, which is not a good bracket sequence.

$S$immediately after processing the $7$th query is `(()`, which is not a good bracket sequence.

$S$immediately after processing the $8$th query is `(())`, which is a good bracket sequence.
</p>

</section>

</div>

</span>

</span>

</div>
