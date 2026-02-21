
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence $A=(A_1,A_2,\ldots,A_N)$of length $N$.
</p>

<p>
Find the maximum length of a subsequence $B=(B_1,B_2,\ldots,B_{|B|})$of integer sequence $A$that satisfies the following condition.
</p>

<ul>

<li>
$B_i+1=B_{i+1}$for all integers $i$satisfying $1\le i\le |B| - 1$.
</li>

</ul>

<details>

<summary>
What is a subsequence
</summary>
A subsequence of sequence $A$is a sequence obtained by choosing zero or more elements of $A$to delete, and arranging the remaining elements in their original order.

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le 2\times 10^5$
</li>

<li>
$1\le A_i\le 10^9$
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

$N$$A_1$$A_2$$\ldots$$A_N$
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

7
3 4 3 5 7 6 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4

</div>

<p>
$B=(3,4,5,6)$is a subsequence of $A$that satisfies the condition, and its length is $4$.
</p>

<p>
There is no subsequence satisfying the condition with length greater than $4$, so output $4$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
5 4 3 2 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10
1 2 3 4 5 6 7 8 9 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

10

</div>

</section>

</div>

</span>

</span>

</div>
