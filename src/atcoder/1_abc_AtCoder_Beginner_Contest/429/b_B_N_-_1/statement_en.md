
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
You are given an integer sequence of length $N$, $A=(A_1,A_2,\ldots,A_N)$, and an integer $M$.
</p>

<p>
Determine whether it is possible to remove one of the $N$elements of $A$so that the sum of the remaining $(N-1)$elements is exactly $M$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\le N\le 100$
</li>

<li>
$0\le M\le 10000$
</li>

<li>
$0\le A_i\le 100$
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

$N$$M$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If it is possible to remove one of the $N$elements of $A$so that the sum of the remaining $(N-1)$elements is exactly $M$, print `Yes`; otherwise, print `No`.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 10
3 2 3 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes

</div>

<p>
If you choose $A_1,A_3,A_4$, the sum is $3+3+4=10$. Therefore, print `Yes`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 16
3 3 4 2 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No

</div>

<p>
No matter how you choose four elements, their sum is not equal to $16$. Therefore, print `No`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

6 16
0 8 0 2 6 8

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

Yes

</div>

</section>

</div>

</span>

</span>

</div>
