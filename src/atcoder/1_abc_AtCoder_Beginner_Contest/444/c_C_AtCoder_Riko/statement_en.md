
<div>

<span>

<span>

<p>
Score : $350$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a sequence of $N$positive integers $A=(A_1,A_2,\dots,A_N)$.
</p>

<p>
Find all positive integers $L$for which the following can occur:
</p>

<blockquote>

<p>
AtCoder Inc. has released a stick-shaped snack called "AtCoderiko."
A cup contains one or more AtCoderikos, each of length $L$.
When Takahashi shook the cup, each AtCoderiko ended up in one of the following states:

</p>

<ul>

<li>
It remained as one AtCoderiko of length $L$. 
</li>

<li>
It broke into two AtCoderikos whose lengths sum to $L$. Here, the length of each AtCoderiko is a positive integer.
</li>

</ul>
After shaking the cup, there were $N$AtCoderikos in the cup, and the length of the $i$-th AtCoderiko was $A_i$.
<p>

</p>

</blockquote>

<p>
The given input guarantees that there exists at least one positive integer $L$for which this can occur.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 3 \times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^9$
</li>

<li>
There exists at least one $L$satisfying the condition.
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
Output all values of $L$satisfying the condition in ascending order, separated by spaces, in one line.
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
10 5 5 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

10 15

</div>

<p>
If the cup initially contained three AtCoderikos of length $10$, and one of them broke into two AtCoderikos of length $5$, the condition is satisfied.

If the cup initially contained two AtCoderikos of length $15$, and each of them broke into two AtCoderikos of lengths $5$and $10$, the condition is satisfied.

No other values of $L$satisfy the condition.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
4 4 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

4

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

6
10 187 344 100 434 257

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

444

</div>

</section>

</div>

</span>

</span>

</div>
