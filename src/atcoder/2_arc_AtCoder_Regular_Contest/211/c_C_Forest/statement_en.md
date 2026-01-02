
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a positive integer $N$, a string $S$of length $N$consisting of `#`and `.`, and a length-$N$sequence of positive integers $R=(R_1,R_2,\dots,R_N)$.
</p>

<p>
There is a forest with $N$sections arranged in a single horizontal line. The sections are numbered $1,2,\dots,N$from left to right.
</p>

<p>
Some sections have trees. Specifically, section $i$has a tree if and only if the $i$-th character of $S$is `#`. It is guaranteed that the following operation can be performed at least once.
</p>

<p>
You can repeat the following operation as many times as you like:
</p>

<ul>

<li>
Choose two sections without trees. Let sections $i$and $j$(where $i < j$) be the chosen sections from left to right. Then, all trees between sections $i$and $j$are removed, and you gain a reward of $R_i+R_j$.
</li>

</ul>

<p>
Here, you cannot perform an operation that removes no trees.
</p>

<p>
Find the number of ways to perform the 
<strong>
first
</strong>
operation to achieve the maximum possible total reward. Two ways are considered distinct if and only if there exists a section chosen in one way but not in the other.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3\leq N\leq 2\times 10^5$
</li>

<li>
The length of $S$is $N$, and each character is `#`or `.`.
</li>

<li>
$1\leq R_i\leq 10^9$$(1\leq i\leq N)$
</li>

<li>
The operation can be performed at least once.
</li>

<li>
$N$and $R_i$are integers.
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

$N$$S$$R_1$$R_2$$\dots$$R_N$
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

8
...###..
20 25 1 1 30 2 1 1

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
There are six ways to perform the first operation, as follows:
</p>

<ul>

<li>
Choose sections $1$and $7$. The trees at sections $4,5,6$are removed, and you gain a reward of $21$.
</li>

<li>
Choose sections $1$and $8$. The trees at sections $4,5,6$are removed, and you gain a reward of $21$.
</li>

<li>
Choose sections $2$and $7$. The trees at sections $4,5,6$are removed, and you gain a reward of $26$.
</li>

<li>
Choose sections $2$and $8$. The trees at sections $4,5,6$are removed, and you gain a reward of $26$.
</li>

<li>
Choose sections $3$and $7$. The trees at sections $4,5,6$are removed, and you gain a reward of $2$.
</li>

<li>
Choose sections $3$and $8$. The trees at sections $4,5,6$are removed, and you gain a reward of $2$.
</li>

</ul>

<p>
No matter which operation is performed, all trees are removed, so a second operation cannot be performed. The maximum possible total reward is $26$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
.#.#.
211 182 192 182 211

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

2

</div>

<p>
The maximum possible total reward is $825$.
</p>

<p>
Note that the goal is not to maximize the reward obtained in the first operation. If you choose sections $1$and $5$first, you can gain a reward of $422$, but no operation can be performed afterwards, and the total reward cannot reach $825$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

11
#..#.##.#..
192 192 192 211 182 192 182 192 182 211 182

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

3

</div>

</section>

</div>

</span>

</span>

</div>
