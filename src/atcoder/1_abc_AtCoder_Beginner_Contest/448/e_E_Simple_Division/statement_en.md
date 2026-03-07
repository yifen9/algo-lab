
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given integers $N$and $M$. Find the remainder when $\lfloor N/M \rfloor$is divided by $\color{red}{10007}$.

Here, $\lfloor x \rfloor$denotes the largest integer not exceeding $x$. For example, $\lfloor 3.14 \rfloor=3$and $\lfloor 10 \rfloor = 10$.
</p>

<p>
In this problem, $N$is not given directly; instead, it is given in run-length encoded form.

Specifically, $N$is represented by a sequence of $K$pairs of a digit $c_i$and an integer $l_i$.

To recover the original $N$, use the following procedure.
</p>

<ul>

<li>
Initially, let string $S$be the empty string.
</li>

<li>
For $i=1,2,\dots,K$, repeat the following.
<ul>

<li>
Append $l_i$copies of digit $c_i$to the end of $S$.
</li>

</ul>

</li>

<li>
Interpret the final $S$as a single integer; that integer is $N$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le M \le 10^4$
</li>

<li>
$1 \le K \le 10^5$
</li>

<li>
$c_i$is one of the digits $0,1,2,3,4,5,6,7,8,9$.
</li>

<li>
$1 \le l_i \le 10^9$
</li>

<li>
$c_1 \neq 0$
</li>

<li>
$M,K,l_i$are integers.
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

$K$$M$$c_1$$l_1$$c_2$$l_2$$\vdots$$c_K$$l_K$
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

6 7
3 1
1 1
6 1
2 2
7 2
6 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3797

</div>

<p>
In this input, $N=316227766$and $M=7$.

$\lfloor 316227766/7 \rfloor = 45175395$, and the remainder when this is divided by $10007$is $3797$, which is the final answer.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1 1
1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10 9999
9 419921892
9 923650333
6 476449815
1 8837775
2 141135534
5 462618481
3 202652735
0 771538044
4 321458589
0 570032864

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

8437

</div>

</section>

</div>

</span>

</span>

</div>
