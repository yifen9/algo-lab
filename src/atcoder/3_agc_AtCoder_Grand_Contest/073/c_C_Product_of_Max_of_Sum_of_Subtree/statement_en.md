
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
There is a tree with $N$vertices numbered from $1$to $N$, where the $i$-th edge connects vertices $A_i$and $B_i$.
</p>

<p>
We will now randomly write real numbers between $-(N-1)$and $1$(inclusive) on each vertex of this tree.
The random number distributions are all independent uniform distributions.
</p>

<p>
Then, the 
<strong>
score
</strong>
of the tree is defined as follows:
</p>

<ul>

<li>
For each vertex $i$, define $x_i$as follows:
<ul>

<li>
The maximum value of the sum of values written on vertices of connected subgraphs that contain vertex $i$
</li>

</ul>

</li>

<li>
If there exists $i$that does not satisfy $0 \leq x_i \leq 1$, the tree's score is $0$.
</li>

<li>
Otherwise, the tree's score is $\prod_{1 \leq i \leq N} x_i$.
</li>

</ul>

<p>
Find the expected value $\text{mod }{998244353}$of the tree's score.
</p>

<details>

<summary>
Definition of expected value $\text{mod }{998244353}$
</summary>

<p>
It can be proved that the sought expected value is always a rational number. Also, under the constraints of this problem, it can be proved that when the value is expressed as an irreducible fraction $\frac{P}{Q}$, we have $Q \neq 0 \pmod{998244353}$. Therefore, an integer $R$satisfying $R \times Q \equiv P \pmod{998244353}, 0 \leq R < 998244353$is uniquely determined. Answer this $R$.


</p>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 5000$
</li>

<li>
$1 \leq A_i, B_i \leq N$
</li>

<li>
The input graph is a tree.
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

$N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_{N-1}$$B_{N-1}$
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

1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

499122177

</div>

<p>
The expected value of the score is $1/2$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

873463809

</div>

<p>
The expected value of the score is $1/8$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

3
1 2
2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

842653798

</div>

<p>
The expected value of the score is $13/648$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

5
1 2
2 3
3 4
4 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

132050425

</div>

<p>
The expected value of the score is $41/187500$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 5**

<div>

8
1 2
1 3
1 4
1 5
5 6
5 7
5 8

</div>

</section>

</div>

<div>

<section>

### **Sample Output 5**

<div>

243711918

</div>

<p>
The expected value of the score is $2477/30064771072$.
</p>

</section>

</div>

</span>

</span>

</div>
