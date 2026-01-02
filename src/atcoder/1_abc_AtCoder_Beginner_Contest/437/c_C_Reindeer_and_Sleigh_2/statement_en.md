
<div>

<span>

<span>

<p>
Score : $350$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$reindeer and one sled. The $i$-th reindeer has weight $W_i$and strength $P_i$.
</p>

<p>
For each reindeer, choose either "pull the sled" or "ride on the sled".
Here, the total strength of the reindeer pulling the sled must be greater than or equal to the total weight of the reindeer riding on the sled.
What is the maximum number of reindeer that can ride on the sled?
</p>

<p>
You are given $T$test cases. Solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq T\leq 10^5$
</li>

<li>
$1\leq N\leq 3\times 10^5$
</li>

<li>
$1\leq W_i,P_i\leq 10^9$
</li>

<li>
All input values are integers.
</li>

<li>
The sum of $N$in one input file is at most $3\times 10^5$.
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
Each test case is given in the following format:
</p>

<div>

$N$$W_1$$P_1$$W_2$$P_2$$\vdots$$W_N$$P_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line should contain the answer for the $i$-th test case.
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
3
3 1
4 1
5 9
5
1000000000 1
1000000000 1
1000000000 1
1000000000 1
1000000000 1
10
133180711 458704923
531424946 225863856
141986070 637075158
500770732 289806469
502866767 408857335
559714289 569084545
287444582 992432993
559747907 753133304
432846188 949871298
727072164 756020367

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
0
6

</div>

<p>
For the 1st test case, if the 3rd reindeer pulls the sled and the 1st and 2nd reindeer ride on the sled, the total strength of the reindeer pulling the sled is $P_3=9$, and the total weight of the reindeer riding on the sled is $W_1+W_2=7$, satisfying the condition. Since not all reindeer can ride on the sled, the answer is $2$.
</p>

</section>

</div>

</span>

</span>

</div>
