
<div>

<span>

<span>

<p>
Score: $250$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You have an empty sequence and $N$balls. The size of the $i$-th ball $(1 \leq i \leq N)$is $2^{A_i}$.
</p>

<p>
You will perform $N$operations.

In the $i$-th operation, you add the $i$-th ball to the right end of the sequence, and repeat the following steps:
</p>

<ol>

<li>
If the sequence has one or fewer balls, end the operation.
</li>

<li>
If the rightmost ball and the second rightmost ball in the sequence have 
<strong>
different
</strong>
sizes, end the operation.
</li>

<li>
If the rightmost ball and the second rightmost ball in the sequence have the 
<strong>
same
</strong>
size, remove these two balls and add a new ball to the right end of the sequence with a size equal to the sum of the sizes of the two removed balls. Then, go back to step 1 and repeat the process.
</li>

</ol>

<p>
Determine the number of balls remaining in the sequence after the $N$operations.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$0 \leq A_i \leq 10^9$
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
Print the number of balls in the sequence after the $N$operations.
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
2 1 1 3 5 3 3

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
The operations proceed as follows:
</p>

<ul>

<li>
After the first operation, the sequence has one ball, of size $2^2$.
</li>

<li>
After the second operation, the sequence has two balls, of sizes $2^2$and $2^1$in order.
</li>

<li>
After the third operation, the sequence has one ball, of size $2^3$. This is obtained as follows:
<ul>

<li>
When the third ball is added during the third operation, the sequence has balls of sizes $2^2, 2^1, 2^1$in order.
</li>

<li>
The first and second balls from the right have the same size, so these balls are removed, and a ball of size $2^1 + 2^1 = 2^2$is added. Now, the sequence has balls of sizes $2^2, 2^2$.
</li>

<li>
Again, the first and second balls from the right have the same size, so these balls are removed, and a ball of size $2^2 + 2^2 = 2^3$is added, leaving the sequence with a ball of size $2^3$.
</li>

</ul>

</li>

<li>
After the fourth operation, the sequence has one ball, of size $2^4$.
</li>

<li>
After the fifth operation, the sequence has two balls, of sizes $2^4$and $2^5$in order.
</li>

<li>
After the sixth operation, the sequence has three balls, of sizes $2^4$, $2^5$, $2^3$in order.
</li>

<li>
After the seventh operation, the sequence has three balls, of sizes $2^4$, $2^5$, $2^4$in order.
</li>

</ul>

<p>
Therefore, you should print $3$, the final number of balls in the sequence.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
0 0 0 1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

4

</div>

<p>
The operations proceed as follows:
</p>

<ul>

<li>
After the first operation, the sequence has one ball, of size $2^0$.
</li>

<li>
After the second operation, the sequence has one ball, of size $2^1$.
</li>

<li>
After the third operation, the sequence has two balls, of sizes $2^1$and $2^0$in order.
</li>

<li>
After the fourth operation, the sequence has three balls, of sizes $2^1$, $2^0$, $2^1$in order.
</li>

<li>
After the fifth operation, the sequence has four balls, of sizes $2^1$, $2^0$, $2^1$, $2^2$in order.
</li>

</ul>

<p>
Therefore, you should print $4$, the final number of balls in the sequence.
</p>

</section>

</div>

</span>

</span>

</div>
