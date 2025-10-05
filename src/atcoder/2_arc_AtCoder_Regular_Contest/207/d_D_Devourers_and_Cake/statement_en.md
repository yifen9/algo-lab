
<div>

<span>

<span>

<p>
Score : $800$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<p>
Taro the First and Jiro the Second bought a rectangular cake as a present for their mother.
They were hungry, so they decided to eat all of the cake except for one piece for their mother.
</p>

</blockquote>

<p>
There is a cake consisting of pieces arranged in $N$rows and $M$columns.
The piece at the $i$-th row from the top and $j$-th column from the left has a strawberry on it when $s_{i,j}$is `1`, and does not have a strawberry when it is `0`.
</p>

<p>
Starting with Taro the First, the two alternately perform an operation on the cake until only one piece remains.
The operations they can perform are as follows. However, they cannot perform an operation that eats all remaining pieces.
</p>

<ul>

<li>
Eat all pieces in the first row from the top
</li>

<li>
Eat all pieces in the first row from the bottom
</li>

<li>
Eat all pieces in the first column from the left
</li>

<li>
Eat all pieces in the first column from the right
</li>

</ul>

<p>
Taro the First wants to leave a piece with a strawberry, and Jiro the Second wants to leave a piece without a strawberry.
Determine whether Taro the First can leave a piece with a strawberry no matter how Jiro the Second operates, when Taro operates appropriately.
</p>

<p>
You are given $T$test cases; find the answer for each of them.
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
$1 \le N,M \le 10^{3}$
</li>

<li>
$1<NM$
</li>

<li>
$s_{i}$is a string of length $M$consisting of `0`and `1`.
</li>

<li>
The sum of $NM$over all test cases is at most $10^6$.
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

$N$$M$$s_1$$s_2$$\vdots$$s_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $T$lines.
</p>

<p>
On the $i$-th line, for the $i$-th test case, print `First`if Taro the First can leave a piece with a strawberry no matter how Jiro the Second operates when Taro operates appropriately, and `Second`otherwise.
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
2 2
01
10
1 4
0100
4 1
0
1
0
0
5 5
00000
11100
01011
00100
01101

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Second
First
First
Second

</div>

<p>
For the first test case, no matter what operation Taro performs, Jiro can leave a piece without a strawberry.
</p>

<p>
For the second test case, if Taro operates appropriately, he can leave a piece with a strawberry no matter how Jiro operates.
</p>

<p>
Note that they cannot choose an operation that eats all remaining pieces.
</p>

</section>

</div>

</span>

</span>

</div>
