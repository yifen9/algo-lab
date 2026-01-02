
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Takahashi has decided to fly in the sky with balloons. Takahashi is at altitude $H$at time $0$(the unit is seconds), and will fly for $10^9$seconds from now.  
</p>

<p>
Takahashi can change his flying altitude by up to $1$per second. However, he cannot make his altitude $0$or less.
</p>

<ul>

<li>
In other words, if $F(t)$denotes Takahashi's altitude at time $t$, then $F(t)$satisfies all of the following conditions:
<ul>

<li>
$F(0) = H$
</li>

<li>
$-1 \leq \dfrac{F(u) - F(t)}{u - t} \leq 1$for $0 \leq t \lt u \leq 10^9$.
</li>

<li>
$F(t) \gt 0$for $0 \leq t \leq 10^9$.
</li>

</ul>

</li>

</ul>

<p>
There are $N$goals regarding altitude. The $i$-th goal is to make the altitude at time $t_i$at least $l_i$and at most $u_i$.

Is it possible for Takahashi to fly in a way that achieves all goals?
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
$1 \leq N \leq 10^5$
</li>

<li>
$1 \leq H \leq 10^9$
</li>

<li>
$1 \leq t_1 \lt t_2 \lt \dots \lt t_N \leq 10^9$
</li>

<li>
$1 \leq l_i \leq u_i \leq 10^9$
</li>

<li>
The sum of $N$over all test cases is at most $10^5$.
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
The input is given from Standard Input in the following format, where $\mathrm{case}_i$denotes the $i$-th test case.
</p>

<div>

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$H$$t_1$$l_1$$u_1$$t_2$$l_2$$u_2$$\vdots$$t_N$$l_N$$u_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line should contain `Yes`if it is possible to fly in a way that achieves all goals in the $i$-th test case, and `No`otherwise.
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
2 5
3 1 4
8 9 11
2 6
1 1 4
3 5 8
10 36
27 37 38
30 34 54
38 20 77
45 1 36
49 38 51
52 31 58
65 43 60
71 14 42
73 36 38
85 14 29

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
No
Yes

</div>

<p>
For the first test case, Takahashi can achieve all goals by flying as follows:
</p>

<ul>

<li>
At time $0$, he is at altitude $5$.
</li>

<li>
From time $0$to time $2$, he descends at a rate of $0.5$per second.
</li>

<li>
At time $2$, he is at altitude $5 - 0.5 \times 2 = 4$.
</li>

<li>
From time $2$to time $3$, he stays at the same altitude.
</li>

<li>
At time $3$, he is at altitude $4$. He satisfies the first goal.
</li>

<li>
From time $3$to time $8$, he ascends at a rate of $1$per second.
</li>

<li>
At time $8$, he is at altitude $4 + 1 \times 5 = 9$. He satisfies the second goal.
</li>

</ul>

<p>
For the second test case, he cannot achieve all goals no matter how he flies.
</p>

</section>

</div>

</span>

</span>

</div>
