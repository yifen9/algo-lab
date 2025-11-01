
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
You are given an integer $N$and a string $S$of length $N-1$consisting of `L`and `R`.
</p>

<p>
Consider writing integers into $N$cells arranged in a row so that the following conditions are satisfied:
</p>

<ul>

<li>
Every cell has one integer written on it.
</li>

<li>
Every integer $1,2,\dots,N$appears in exactly one cell.
</li>

<li>
When the $i$-th character of $S$is `L`, $i+1$is written to the left of $i$.
</li>

<li>
When the $i$-th character of $S$is `R`, $i+1$is written to the right of $i$.
</li>

</ul>

<p>
Let $C_i$be the number of integers that can be written in the $i$-th cell from the left.
Find $C_1,C_2,\dots,C_N$.
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
$1 \le T \le 20000$
</li>

<li>
$2 \le N \le 3 \times 10^5$
</li>

<li>
$S$is a string of length $N-1$consisting of `L`and `R`.
</li>

<li>
For a single input, the sum of $N$does not exceed $3 \times 10^5$.
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

$N$$S$
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
The $i$-th line should contain the answer for the $i$-th test case in the following format:
</p>

<div>

$C_1$$C_2$$\dots$$C_N$
</div>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5
5
RLLR
3
RL
2
L
3
RR
20
RLLLLLLLLRLRRLLLRLR

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2 4 3 4 2
2 2 1
1 1
1 1 1
5 9 13 14 15 17 18 19 19 20 20 19 19 18 17 16 14 12 9 5

</div>

<p>
This input contains five test cases.
</p>

<ul>

<li>
For the first test case, there are $11$possible ways to fill the cells as follows:
<ul>

<li>
$(1,4,3,2,5)$
</li>

<li>
$(1,4,3,5,2)$
</li>

<li>
$(1,4,5,3,2)$
</li>

<li>
$(4,1,3,2,5)$
</li>

<li>
$(4,1,3,5,2)$
</li>

<li>
$(4,1,5,3,2)$
</li>

<li>
$(4,3,1,2,5)$
</li>

<li>
$(4,3,1,5,2)$
</li>

<li>
$(4,3,5,1,2)$
</li>

<li>
$(4,5,1,3,2)$
</li>

<li>
$(4,5,3,1,2)$
</li>

</ul>

</li>

<li>
From this, each value of $C_i$is determined as follows:
<ul>

<li>
The integers that can be written in the $1$-st cell from the left are $1,4$, which is two integers.
</li>

<li>
The integers that can be written in the $2$-nd cell from the left are $1,3,4,5$, which is four integers.
</li>

<li>
The integers that can be written in the $3$-rd cell from the left are $1,3,5$, which is three integers.
</li>

<li>
The integers that can be written in the $4$-th cell from the left are $1,2,3,5$, which is four integers.
</li>

<li>
The integers that can be written in the $5$-th cell from the left are $2,5$, which is two integers.
</li>

</ul>

</li>

<li>
For the second test case, there are two possible ways to fill the cells as follows:
<ul>

<li>
$(1,3,2)$
</li>

<li>
$(3,1,2)$
</li>

</ul>

</li>

<li>
For the third test case, there is one possible way to fill the cells as follows:
<ul>

<li>
$(2,1)$
</li>

</ul>

</li>

<li>
For the fourth test case, there is one possible way to fill the cells as follows:
<ul>

<li>
$(1,2,3)$
</li>

</ul>

</li>

</ul>

</section>

</div>

</span>

</span>

</div>
