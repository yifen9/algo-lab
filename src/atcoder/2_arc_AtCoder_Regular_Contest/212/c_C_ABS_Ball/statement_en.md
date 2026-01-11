
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
There are $N$white balls. First, you paint each ball red or blue.
</p>

<p>
Then, you place these $N$red or blue painted balls in one of $M$distinguishable boxes.
</p>

<p>
Let $a_i$and $b_i$be the number of red and blue balls in the $i$-th box, respectively.
</p>

<p>
Find the sum, modulo $998244353$, of $\prod_{1\leq i \le M}|a_i-b_i|$over all ways to place the balls.
</p>

<p>
Here, two ways of placing balls are different if and only if at least one of $a_i$and $b_i$is different for some $i$.
</p>

<p>
Particularly, 
<strong>
balls are not distinguished from each other
</strong>
.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N,M \le  10^7$
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

$N$$M$
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

2 1

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
There are three ways to place balls in box $1$.

If you place one red ball and one blue ball, $|a_1-b_1|=0$.

If you place two red balls or two blue balls, $|a_1-b_1|=2$.

Therefore, the answer is $0 + 2 + 2 = 4$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10000000 5000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

965172629

</div>

</section>

</div>

</span>

</span>

</div>
