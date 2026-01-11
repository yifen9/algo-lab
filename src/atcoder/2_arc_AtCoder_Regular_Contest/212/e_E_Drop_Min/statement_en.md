
<div>

<span>

<span>

<p>
Score : $700$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a permutation $P$of $(1,2,\ldots,N)$and an empty array $A$.
Perform the following operation $N-1$times on $P$:
</p>

<ul>

<li>
Choose two adjacent elements. Remove the smaller of the chosen elements from $P$and concatenate the parts before and after the removed element. Append the removed element to the end of $A$.
</li>

</ul>

<p>
Find the number, modulo $998244353$, of possible final sequences $A$of length $N-1$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \le N \le 2\times 10^5$
</li>

<li>
$1 \le P_i \le N$
</li>

<li>
$P$is a permutation of $(1,2,\ldots,N)$.
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

$N$$P_1$$P_2$$\ldots$$P_N$
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

4
1 2 3 4

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
All six permutations of $(1,2,3)$are possible as the final $A$.
</p>

<p>
For example, $A=(2,1,3)$can be obtained as follows:
</p>

<ul>

<li>
Choose $2,3$. Remove $2$, and now $P=(1,3,4), A=(2)$.
</li>

<li>
Choose $1,3$. Remove $1$, and now $P=(3,4), A=(2,1)$.
</li>

<li>
Choose $3,4$. Remove $3$, and now $P=(4), A=(2,1,3)$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
3 1 2

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

24
10 24 3 4 8 14 5 2 22 9 21 1 15 6 13 23 18 12 7 17 19 16 20 11

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

303178128

</div>

</section>

</div>

</span>

</span>

</div>
