
<div>

<span>

<span>

<p>
Score : $1000$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a sequence of positive integers $A=(A_1,A_2,\ldots,A_N)$.
</p>

<p>
There are $2^N$subsequences of $A$when distinguishing subsequences by the indices of their elements. Let $S_1, S_2, \ldots, S_{2^N}$be the sums of these subsequences, enumerated 
<strong>
in ascending order
</strong>
.
</p>

<p>
For all integers $k$($1\leq k\leq 2^N-1$) that satisfy $1.01 \times S_k\leq S_{k+1}$, output $S_k, S_{k+1}, (k\bmod 998244353)$.
</p>

<details>

<summary>
What is a subsequence
</summary>
A subsequence of a sequence $A$is a sequence obtained by removing zero or more elements from $A$and arranging the remaining elements in their original order.

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\leq N\leq 5000$
</li>

<li>
$1\leq A_i\leq 10^{13}$
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
On the first line, output the number of integers $k$that satisfy the condition.
</p>

<p>
From the second line onwards, for each integer $k$that satisfies the condition, output $S_k, S_{k+1}, (k\bmod 998244353)$separated by spaces on each line.
</p>

<p>
Output in ascending order of $k$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
5 5 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

5
0 3 1
3 5 2
5 8 4
8 10 6
10 13 7

</div>

<p>
We have the following eight subsequences:
</p>

<ul>

<li>
The empty subsequence. The sum is $0$.
</li>

<li>
$(5)$. The sum is $5$. This subsequence appears twice.
</li>

<li>
$(3)$. The sum is $3$.
</li>

<li>
$(5,5)$. The sum is $10$.
</li>

<li>
$(5,3)$. The sum is $8$. This subsequence appears twice.
</li>

<li>
$(5,5,3)$. The sum is $13$.
</li>

</ul>

<p>
$S_1, S_2, \ldots, S_8$are $0,3,5,5,8,8,10,13$in order.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2
100 101

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

3
0 100 1
100 101 2
101 201 3

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

2
101 102

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

2
0 101 1
102 203 3

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

20
456 206 448 830 937 793 483 527 772 239 361 925 364 956 355 420 557 739 323 912

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

23
0 206 1
206 239 2
239 323 3
323 355 4
355 361 5
364 420 7
420 445 8
448 456 10
456 483 11
483 527 12
529 557 14
570 594 19
594 600 20
603 626 22
626 654 23
662 678 26
695 716 32
725 733 36
743 763 39
784 793 48
820 830 60
850 865 65
11397 11603 1048575

</div>

</section>

</div>

</span>

</span>

</div>
