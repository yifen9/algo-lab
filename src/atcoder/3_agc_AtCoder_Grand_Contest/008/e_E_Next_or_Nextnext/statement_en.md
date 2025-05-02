
<div>

<span>

<span>

<p>
Score : $1400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence $a$of length $N$.
How many permutations $p$of the integers $1$through $N$satisfy the following condition?
</p>

<ul>

<li>
For each $1 ≤ i ≤ N$, at least one of the following holds: $p_i = a_i$and $p_{p_i} = a_i$.
</li>

</ul>

<p>
Find the count modulo $10^9 + 7$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 ≤ N ≤ 10^5$
</li>

<li>
$a_i$is an integer.
</li>

<li>
$1 ≤ a_i ≤ N$
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

$N$$a_1$$a_2$$...$$a_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the number of the permutations $p$that satisfy the condition, modulo $10^9 + 7$.
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
1 2 3

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
The following four permutations satisfy the condition:
</p>

<ul>

<li>
$(1, 2, 3)$
</li>

<li>
$(1, 3, 2)$
</li>

<li>
$(3, 2, 1)$
</li>

<li>
$(2, 1, 3)$
</li>

</ul>

<p>
For example, $(1, 3, 2)$satisfies the condition because $p_1 = 1$, $p_{p_2} = 2$and $p_{p_3} = 3$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2
1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

<p>
The following one permutation satisfies the condition:
</p>

<ul>

<li>
$(2, 1)$
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

3
2 1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

2

</div>

<p>
The following two permutations satisfy the condition:
</p>

<ul>

<li>
$(2, 3, 1)$
</li>

<li>
$(3, 1, 2)$
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

3
1 1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 5**

<div>

13
2 1 4 3 6 7 5 9 10 8 8 9 11

</div>

</section>

</div>

<div>

<section>

### **Sample Output 5**

<div>

6

</div>

</section>

</div>

</span>

</span>

</div>
