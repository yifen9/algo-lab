
<div>
﻿
<span>

<span>

<p>
Score : $525$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a length-$N$integer sequence $A=(A _ 1,A _ 2,\ldots,A _ N)$.
</p>

<p>
There are $2 ^ N$(not necessarily contiguous) subsequences of $A$.
Find how many subsequences $(A _ {i _ 1},A _ {i _ 2},\ldots,A _ {i _ k})\ (1\le i _ 1\lt i _ 2\lt\cdots\lt i _ k\le N)$satisfy both of the following two conditions:
</p>

<ul>

<li>
The selected elements are not adjacent in $A$. That is, $1+i _ j\ne i _ {j+1}$holds for all $1\le j\lt k$.
</li>

<li>
The sum is a multiple of $M$. That is, $\displaystyle\sum _ {j=1} ^ kA _ {i _ j}\equiv0\pmod M$.
</li>

</ul>

<p>
Even if two subsequences are equal as integer sequences, they are counted separately if the positions from which they are taken are different.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le60$
</li>

<li>
$1\le M\le10 ^ 9$
</li>

<li>
$0\le A _ i\lt M$
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

$N$$M$$A _ 1$$A _ 2$$\ldots$$A _ N$
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

7 6
3 1 4 1 5 3 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

6

</div>

<p>
The following six subsequences satisfy the conditions:
</p>

<ul>

<li>
$()=()$
</li>

<li>
$(A _ 1,A _ 3,A _ 5)=(3,4,5)$
</li>

<li>
$(A _ 1,A _ 4,A _ 7)=(3,1,2)$
</li>

<li>
$(A _ 1,A _ 6)=(3,3)$
</li>

<li>
$(A _ 2,A _ 5)=(1,5)$
</li>

<li>
$(A _ 3,A _ 7)=(4,2)$
</li>

</ul>

<p>
Thus, print `6`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

15 10
5 5 5 5 5 5 5 5 5 5 5 5 5 5 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

798

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

20 998244353
778718481 719092922 676292280 713825156 0 434453766 620370916 67922064 0 577696866 21516423 955580612 955580612 0 332156721 0 0 0 632133714 500614291

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

40

</div>

</section>

</div>

</span>

</span>

</div>
