
<div>

<span>

<span>

<p>
Score : $475$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a sequence of positive integers $A=(A_1,A_2,\dots,A_N)$of length $N$.
</p>

<p>
For each $k=1,2,\dots,N$, find the remainder when the least common multiple of the $N-1$elements of $A$excluding $A_k$is divided by $998244353$.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq 10^5$
</li>

<li>
$2 \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^7$
</li>

<li>
All input values are integers.
</li>

<li>
The sum of $N$over all test cases in a single input is at most $2 \times 10^5$.
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Here, $\mathrm{case}_i$denotes the input for the $i$-th test case. Each test case is given in the following format:
</p>

<div>

$N$$A_1$$A_2$$\cdots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output in the following format:
</p>

<div>

$\mathrm{answer}_1$$\mathrm{answer}_2$$\vdots$$\mathrm{answer}_T$
</div>

<p>
Here, $\mathrm{answer}_i$denotes the output for the $i$-th test case.
For each test case, output as follows.
</p>

<p>
Let $L_k$be the remainder when the least common multiple of the $N-1$elements of $A$excluding $A_k$is divided by $998244353$.
Then, output in the following format:
</p>

<div>

$L_1$$L_2$$\cdots$$L_N$
</div>

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
9 12 25 8 15
8
592 26 167 912 171 321 327 651
10
9566582 2785103 1924635 359502 6912831 4893928 2820155 5071742 1836019 9037883

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

600 1800 360 900 1800
447582749 506009091 523568328 588652065 196217355 471970745 921220985 738745385
747032704 756838459 344127037 146466685 159487731 555429485 826726159 884617928 322846201 298477407

</div>

<p>
For the first test case, the following holds.
</p>

<ul>

<li>
The $N-1$elements of $A$excluding $A_1$are $12,25,8,15$, and their least common multiple is $600$.
</li>

<li>
The $N-1$elements of $A$excluding $A_2$are $9,25,8,15$, and their least common multiple is $1800$.
</li>

<li>
The $N-1$elements of $A$excluding $A_3$are $9,12,8,15$, and their least common multiple is $360$.
</li>

<li>
The $N-1$elements of $A$excluding $A_4$are $9,12,25,15$, and their least common multiple is $900$.
</li>

<li>
The $N-1$elements of $A$excluding $A_5$are $9,12,25,8$, and their least common multiple is $1800$.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
