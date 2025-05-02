
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
The 
<em>
ABC number
</em>
of a string $T$is the number of triples of integers $(i, j, k)$that satisfy all of the following conditions:
</p>

<ul>

<li>
$1 ≤ i < j < k ≤ |T|$($|T|$is the length of $T$.)
</li>

<li>
$T_i =$`A`($T_i$is the $i$-th character of $T$from the beginning.)
</li>

<li>
$T_j =$`B`
</li>

<li>
$T_k =$`C`
</li>

</ul>

<p>
For example, when $T =$`ABCBC`, there are three triples of integers $(i, j, k)$that satisfy the conditions: $(1, 2, 3), (1, 2, 5), (1, 4, 5)$. Thus, the ABC number of $T$is $3$.
</p>

<p>
You are given a string $S$. Each character of $S$is `A`, `B`, `C`or `?`.
</p>

<p>
Let $Q$be the number of occurrences of `?`in $S$. We can make $3^Q$strings by replacing each occurrence of `?`in $S$with `A`, `B`or `C`. Find the sum of the ABC numbers of all these strings.
</p>

<p>
This sum can be extremely large, so print the sum modulo $10^9 + 7$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3 ≤ |S| ≤ 10^5$
</li>

<li>
Each character of $S$is `A`, `B`, `C`or `?`.
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
Input is given from Standard Input in the following format:
</p>

<div>

$S$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the sum of the ABC numbers of all the $3^Q$strings, modulo $10^9 + 7$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

A??C

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

8

</div>

<p>
In this case, $Q = 2$, and we can make $3^Q = 9$strings by by replacing each occurrence of `?`with `A`, `B`or `C`. The ABC number of each of these strings is as follows:
</p>

<ul>

<li>
`AAAC`: $0$
</li>

<li>
`AABC`: $2$
</li>

<li>
`AACC`: $0$
</li>

<li>
`ABAC`: $1$
</li>

<li>
`ABBC`: $2$
</li>

<li>
`ABCC`: $2$
</li>

<li>
`ACAC`: $0$
</li>

<li>
`ACBC`: $1$
</li>

<li>
`ACCC`: $0$
</li>

</ul>

<p>
The sum of these is $0 + 2 + 0 + 1 + 2 + 2 + 0 + 1 + 0 = 8$, so we print $8$modulo $10^9 + 7$, that is, $8$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

ABCBC

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
When $Q = 0$, we print the ABC number of $S$itself, modulo $10^9 + 7$. This string is the same as the one given as an example in the problem statement, and its ABC number is $3$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

????C?????B??????A???????

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

979596887

</div>

<p>
In this case, the sum of the ABC numbers of all the $3^Q$strings is $2291979612924$, and we should print this number modulo $10^9 + 7$, that is, $979596887$.
</p>

</section>

</div>

</span>

</span>

</div>
