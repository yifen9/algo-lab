
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

<p>
A store sells $N$items, numbered as item $1$, item $2$, $\ldots$, item $N$. 

Item $i$$(1\leq i\leq N)$has a price of $P_i$yen and a value of $V_i$. The store has only one stock of each item.  
</p>

<p>
Takahashi chooses some items such that the total price is at most $M$yen.

Here, it is guaranteed that $M$is at least the price of any item.
That is, for any $1\leq i\leq N$, there exists a way to choose items such that the total price is at most $M$yen and item $i$is included.
</p>

<p>
For each $1\leq i\leq N$, determine which of the following three categories item $i$falls into:
</p>

<ul>

<li>
Category A: To maximize the total value of the chosen items (while keeping the total price at most $M$yen), that item must be chosen.
</li>

<li>
Category B: To maximize the total value of the chosen items (while keeping the total price at most $M$yen), that item may or may not be chosen.
</li>

<li>
Category C: To maximize the total value of the chosen items (while keeping the total price at most $M$yen), that item must never be chosen.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N\leq 1000$
</li>

<li>
$1\leq M\leq 5\times 10^4$
</li>

<li>
$1\leq P_i\leq M$
</li>

<li>
$1\leq V_i\leq 10^9$
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

$N$$M$$P_1$$V_1$$P_2$$V_2$$\vdots$$P_N$$V_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print a string of length $N$consisting of `A`, `B`, and `C`.

If item $i$$(1\leq i\leq N)$falls into category $X$(where $X$is A, B, or C), the $i$-th character of the output string should be $X$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 7
2 5
2 5
3 5
3 10
3 20

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

BBCBA

</div>

<p>
The maximum possible total value when choosing items such that the total price is at most $7$yen is $30$, which can be achieved by one of the following:
</p>

<ul>

<li>
Choosing items $1$, $2$, and $5$.
</li>

<li>
Choosing items $4$and $5$.
</li>

</ul>

<p>
(There is no other way to choose items such that the total price is at most $7$yen and the total value is $30$.) 

Thus, the category of each item is as follows:
</p>

<ul>

<li>
Item $5$is an item that must be chosen to maximize the total value of the chosen items (category A).
</li>

<li>
Items $1$, $2$, and $4$are items that may or may not be chosen to maximize the total value of the chosen items (category B).
</li>

<li>
Item $3$is an item that must never be chosen to maximize the total value of the chosen items (category C).
</li>

</ul>

<p>
Therefore, according to the output format, print `BBCBA`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

7 3
1 1
1 1
1 2
1 2
1 2
1 3
1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

CCBBBAA

</div>

<p>
The total value is maximized when choosing any one of items $3$, $4$, $5$, along with items $6$and $7$.

Note that even if items have equal prices and values, they are still distinguished as different items.
</p>

</section>

</div>

</span>

</span>

</div>
