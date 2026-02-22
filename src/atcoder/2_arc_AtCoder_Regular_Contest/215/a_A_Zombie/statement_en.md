
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
There is a road of length $L$extending left and right. There are $N$zombies on this road, and the $i$-th zombie is at a distance of $A_i$from the left end of the road.
Here, $L$and all $A_i$are even.
</p>

<p>
You have $K$pieces of bait for the zombies, and you can place a piece of bait at any position on the road, including both ends, at any time.
However, there must never be a moment when two or more pieces of bait exist on the road simultaneously.
When bait exists on the road, each zombie moves toward the bait at a speed of $1$per unit time. When one or more zombies reach the same position as the bait, the bait is eaten and disappears instantly.
</p>

<p>
When no bait exists on the road, zombies do not move.
Find the maximum total amount of time bait exists on the road when the times and positions to place the bait are chosen optimally.
It can be proved that the answer is an integer.
</p>

<p>
You are given $T$test cases; solve each one.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 10^5$
</li>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le K \le 10^9$
</li>

<li>
$2 \le L \le 10^9$
</li>

<li>
$0 \le A_i \le L$
</li>

<li>
$L$is even.
</li>

<li>
All $A_i$are even.
</li>

<li>
The sum of $N$over all test cases is at most $2 \times 10^5$.
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$K$$L$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines.
</p>

<p>
The $i$-th line should contain the maximum total amount of time bait exists on the road for the $i$-th test case.
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
2 2 20
4 18
8 9 14
0 2 4 6 8 10 12 14
3 3 140
120 70 20

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

18
40
160

</div>

<p>
For the first test case, it is optimal to place the bait as follows.
</p>

<ul>

<li>
First, place bait at position $11$. The two zombies simultaneously reach position $11$after $7$units of time and eat the bait.
</li>

<li>
Then, place bait at position $0$. The two zombies simultaneously reach position $0$after $11$units of time and eat the bait.
</li>

</ul>

<p>
The total amount of time bait exists on the road is $7 + 11 = 18$.
</p>

</section>

</div>

</span>

</span>

</div>
