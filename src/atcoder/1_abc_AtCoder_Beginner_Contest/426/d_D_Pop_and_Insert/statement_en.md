
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
You are given a string $S$of length $N$consisting of `0`and `1`.
</p>

<p>
You can perform the following operation on $S$any number of times (possibly zero):
</p>

<ul>

<li>
Delete the first or last character, flip it (change `0`to `1`or `1`to `0`), and insert it back at any position.
More formally, let $r($`0`$)=$`1`and $r($`1`$)=$`0`, and perform one of the following: (Here, $S_i$denotes the $i$-th character of $S$.)
<ul>

<li>
Choose any $i\ (1\leq i\leq N)$and change $S$to $S_2\dots S_i\,r(S_1)\,S_{i+1}\dots S_N$.
</li>

<li>
Choose any $i\ (0\leq i\leq N-1)$and change $S$to $S_1\dots S_i\,r(S_N)\,S_{i+1}\dots S_{N-1}$.
</li>

</ul>

</li>

</ul>

<p>
Find the minimum number of operations required to make all characters of $S$the same.
It can be proved that such a sequence of operations always exists.
</p>

<p>
You are given $T$test cases, so solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq T\leq 2\times 10^5$
</li>

<li>
$2\leq N \leq 5\times 10^5$
</li>

<li>
$T$and $N$are integers.
</li>

<li>
$S$is a string of length $N$consisting of `0`and `1`.
</li>

<li>
The sum of $N$over all test cases is at most $5\times 10^5$.
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
$\text{case}_i$represents the $i$-th test case. Each test case is given in the following format:
</p>

<div>

$N$$S$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line $(1\leq i\leq T)$should contain the answer for the $i$-th test case.
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
5
01001
3
000
15
110010111100101

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4
0
16

</div>

<p>
For the first test case, for example, you can make all characters of $S$into `0`with four operations as follows.
It is impossible to make all characters of $S$the same with three or fewer operations, so the answer is $4$.
</p>

<ul>

<li>
Delete the first character `0`, and insert `1`between the 1st and 2nd characters (in $S$after deletion). $S$becomes `11001`.
</li>

<li>
Delete the first character `1`, and insert `0`between the 2nd and 3rd characters (in $S$after deletion). $S$becomes `10001`.
</li>

<li>
Delete the last character `1`, and insert `0`at the end (in $S$after deletion). $S$becomes `10000`.
</li>

<li>
Delete the first character `1`, and insert `0`at the beginning (in $S$after deletion). $S$becomes `00000`.
</li>

</ul>

<p>
For the second test case, all characters of $S$are the same from the beginning, so no operation is needed.
</p>

</section>

</div>

</span>

</span>

</div>
