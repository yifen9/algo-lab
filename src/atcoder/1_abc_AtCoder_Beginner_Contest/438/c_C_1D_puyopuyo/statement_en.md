
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
You are given an integer sequence $A=(A_1,A_2,\ldots,A_N)$of length $N$.
</p>

<p>
You can perform the following operation zero or more times in any order:
</p>

<ul>

<li>
Choose an integer $k$between $1$and $|A|-3$, inclusive, such that $A_k=A_{k+1}=A_{k+2}=A_{k+3}$, and remove $A_k,A_{k+1},A_{k+2},A_{k+3}$from $A$. (More formally, replace $A$with $(A_1,A_2,\ldots,A_{k-1},A_{k+4},A_{k+5},\ldots,A_N)$.)
</li>

</ul>

<p>
Here, $|A|$represents the length of the integer sequence $A$.
</p>

<p>
Find the minimum possible value of the final $|A|$after repeating the operation.
</p>

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
$1\le A_i\le N$
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
Output the minimum possible value of the final $|A|$after repeating the operation.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

10
1 1 1 4 4 4 4 1 2 3

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
You can make $|A|=2$with two operations as follows:
</p>

<ul>

<li>
Choose $k=4$. This choice is valid since $A_4=A_5=A_6=A_7=4$holds. $A=(1,1,1,1,2,3)$is obtained.
</li>

<li>
Choose $k=1$. This choice is valid since $A_1=A_2=A_3=A_4=1$holds. $A=(2,3)$is obtained.
</li>

</ul>

<p>
It is impossible to make $|A|$less than $2$, so output $2$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
2 1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

3

</div>

<p>
You cannot perform any operation from the beginning.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

13
1 1 4 4 4 1 1 1 1 4 1 4 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

5

</div>

</section>

</div>

</span>

</span>

</div>
