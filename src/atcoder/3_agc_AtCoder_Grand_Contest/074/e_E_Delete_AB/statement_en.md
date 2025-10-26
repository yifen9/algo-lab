
<div>

<span>

<span>

<p>
Score : $1200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
For a string $X = X_1X_2\dots X_{|X|}$and positive integers $l,r~(1 \leq l \leq r \leq |X|)$, let $X_{l,r} = X_l X_{l+1}\dots X_r$. 
</p>

<p>
You are given a string $S=S_1S_2\dots S_{|S|}$consisting of `A`and `B`.

You are given $Q$queries. For each query, answer the following question:
</p>

<ul>

<li>
Starting from the state $T = S_{l,r}$, find the minimum possible length of a palindrome that can be obtained by performing the operation "choose one occurrence of `AB`that appears as a contiguous substring in $T$and delete it" zero or more times.

If no palindrome can be obtained regardless of how the operation is performed, output `-1`.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq |S| \leq 4 \times 10^5$
</li>

<li>
$1 \leq Q \leq 5 \times 10^4$
</li>

<li>
$1 \leq l \leq r \leq |S|$
</li>

<li>
$S$is a string consisting of `A`and `B`.
</li>

<li>
$Q,l,r$are integers.
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

$S$$Q$$\mathrm{Query}_1$$\mathrm{Query}_2$$\vdots$$\mathrm{Query}_Q$
</div>

<p>
$\mathrm{Query}_q$represents the $q$-th query and is given in the following format:
</p>

<div>

$l$$r$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $q$-th line should contain the answer for $\mathrm{Query}_q$.  
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

ABBABB
5
1 6
4 5
3 5
2 3
3 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
0
1
2
-1

</div>

<p>
For the first, second, and third queries, by performing the operation as follows, you can obtain a palindrome with the minimum length among those obtained by the operation.
</p>

<ul>

<li>
`ABBABB`$\rightarrow$`ABBB`$\rightarrow$`BB`
</li>

<li>
`AB`$\rightarrow$(empty string)
</li>

<li>
`BAB`$\rightarrow$`B`
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
