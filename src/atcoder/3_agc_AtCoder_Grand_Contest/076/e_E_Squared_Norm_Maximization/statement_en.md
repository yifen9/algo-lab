
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
You are given $N$pairs of integers $(A_1,B_1),(A_2,B_2),\cdots,(A_N,B_N)$.
</p>

<p>
For a subset $s$of $\{1,2,\cdots,N\}$, we define its 
<strong>
score
</strong>
as follows:
</p>

<ul>

<li>
$(\sum_{i \in s} A_i)^2 + (\sum_{i \in s} B_i)^2 - 3 \sum_{i \in s} (A_i^2+B_i^2)$
</li>

</ul>

<p>
Find the maximum possible value of the score.
</p>

<p>
Solve $T$cases for one input.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq 250000$
</li>

<li>
$1 \leq N \leq 250000$
</li>

<li>
$\sum_{1 \leq i \leq N} |A_i| \leq 10^9$
</li>

<li>
$\sum_{1 \leq i \leq N} |B_i| \leq 10^9$
</li>

<li>
The sum of $N$over the $T$cases is at most $250000$.
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

$T$$case_1$$case_2$$\vdots$$case_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_N$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines.
The $i$-th line should contain the answer for the $i$-th case.
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
4
1 0
0 1
-1 0
0 -1
4
1 0
1 0
1 0
1 0
6
1 -9
-7 -2
0 -10
10 1
2 -8
1 -8
10
19271058 -140039457
-3441379 -134156148
227767903 -70474702
-837477 -74699717
153584327 80404336
115741008 -22141349
-190028077 -21940357
76149725 17176032
159846847 -296045185
-53332199 142922717

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

0
4
296
178262497119089558

</div>

<p>
In the first case, if $s=\{\}$, the score is $0$, which is the maximum.
</p>

<p>
In the second case, if $s=\{1,2,3,4\}$, the score is $4$, which is the maximum.
</p>

</section>

</div>

</span>

</span>

</div>
