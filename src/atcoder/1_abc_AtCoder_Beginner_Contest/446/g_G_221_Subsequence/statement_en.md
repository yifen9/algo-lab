
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
For a sequence $X = (X_1, \dots, X_n)$of positive integers, we call $X$a 
<strong>
221 sequence
</strong>
if and only if the length and value are equal for every (length, value) pair in its run-length encoding. More formally, a sequence satisfying the following condition is called a 221 sequence.
</p>

<ul>

<li>
For any integer pair $(l, r)$satisfying $1 \leq l \leq r \leq n$, if all three of the following conditions hold, then $(r-l+1) = X_l$.
<ul>

<li>
$l = 1$or ($l \geq 2$and $X_{l-1} \neq X_l$)
</li>

<li>
$r = n$or ($r \leq n-1$and $X_{r+1} \neq X_r$)
</li>

<li>
$X_l = X_{l+1} = \dots = X_r$
</li>

</ul>

</li>

</ul>

<p>
For example, $(2,2,3,3,3,1,2,2)$is a 221 sequence, but $(1,1)$and $(4,4,1,4,4)$are not 221 sequences.
</p>

<p>
You are given a sequence $A = (A_1, \dots, A_N)$of positive integers of length $N$. Find the number, modulo $998244353$, of non-empty (not necessarily contiguous) subsequences of $A$that are 221 sequences.
Even if two subsequences are extracted from different positions, they are counted as one if they are equal as sequences.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 500\,000$
</li>

<li>
$1 \leq A_i \leq N$
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

$N$$A_1$$A_2$$\cdots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer on one line.
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
2 1 2 1 1 2 7 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

5

</div>

<p>
The 221 sequences that appear as non-empty subsequences of $A$are the following five:
</p>

<ul>

<li>
$(1)$
</li>

<li>
$(1,2,2)$
</li>

<li>
$(2,2)$
</li>

<li>
$(2,2,1)$
</li>

<li>
$(2,2,1,2,2)$
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
2 3 4 5 4

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
No 221 sequences appear as non-empty subsequences of $A$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

20
2 2 3 1 1 4 1 4 1 4 2 4 1 2 1 4 4 1 1 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

15

</div>

</section>

</div>

</span>

</span>

</div>
