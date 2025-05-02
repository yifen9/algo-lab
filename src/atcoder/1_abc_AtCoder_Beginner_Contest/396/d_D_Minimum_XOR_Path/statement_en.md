
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
You are given a simple connected undirected graph with $N$vertices numbered $1$through $N$and $M$edges numbered $1$through $M$. Edge $i$connects vertices $u_i$and $v_i$, and has a label $w_i$.
</p>

<p>
Among all simple paths (paths that do not pass through the same vertex more than once) from vertex $1$to vertex $N$, find the minimum XOR of the labels of the edges on the path.
</p>

<details>

<summary>
Notes on XOR
</summary>
For non-negative integers $A$and $B$, their XOR $A \oplus B$is defined as follows:


<ul>

<li>
In the binary representation of $A \oplus B$, the digit in the place corresponding to $2^k \,(k \ge 0)$is $1$if and only if exactly one of the digits in the same place of $A$and $B$is $1$; otherwise, it is $0$.
</li>

</ul>
For example, $3 \oplus 5 = 6$(in binary: $011 \oplus 101 = 110$).

In general, the XOR of $k$integers $p_1, \dots, p_k$is defined as $(\cdots ((p_1 \oplus p_2) \oplus p_3) \oplus \cdots \oplus p_k)$. It can be proved that it does not depend on the order of $p_1, \dots, p_k$.


</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 10$
</li>

<li>
$N-1 \leq M \leq \frac{N(N-1)}{2}$
</li>

<li>
$1 \leq u_i < v_i \leq N$
</li>

<li>
$0 \leq w_i < 2^{60}$
</li>

<li>
The given graph is a simple connected undirected graph.
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

$N$$M$$u_1$$v_1$$w_1$$u_2$$v_2$$w_2$$\vdots$$u_M$$v_M$$w_M$
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

4 4
1 2 3
2 4 5
1 3 4
3 4 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3

</div>

<p>
There are two simple paths from vertex $1$to vertex $4$:
</p>

<ul>

<li>
$1 \to 2 \to 4$
</li>

<li>
$1 \to 3 \to 4$
</li>

</ul>

<p>
The XOR of the labels on the edges of the first path is $6$, and that of the second path is $3$. Therefore, the answer is $3$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 3
1 2 1
2 3 2
3 4 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

7

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

7 10
1 2 726259430069220777
1 4 988687862609183408
1 5 298079271598409137
1 6 920499328385871537
1 7 763940148194103497
2 4 382710956291350101
3 4 770341659133285654
3 5 422036395078103425
3 6 472678770470637382
5 7 938201660808593198

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

186751192333709144

</div>

</section>

</div>

</span>

</span>

</div>
