
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
Takahashi and Aoki walk on a two-dimensional plane.
</p>

<p>
Takahashi's start point is $(TS_X, TS_Y)$and goal point is $(TG_X, TG_Y)$.
Aoki's start point is $(AS_X, AS_Y)$and goal point is $(AG_X, AG_Y)$.
</p>

<p>
They simultaneously depart from their respective start points and walk straight toward their respective goal points at speed $1$, and stop when they reach their respective goal points.
(Note that they depart simultaneously, but they do not necessarily stop at the same time.)
</p>

<p>
Find the distance between them at the moment when the distance between them is shortest (including the moment they depart and after they stop).
</p>

<p>
Here, distance refers to Euclidean distance. That is, the distance between two points $(x_1,y_1),(x_2,y_2)$is defined as $\sqrt{(x_1-x_2)^2+(y_1-y_2)^2}$.
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
$-100\leq TS_X,TS_Y,TG_X,TG_Y,AS_X,AS_Y,AG_X,AG_Y \leq 100$
</li>

<li>
$(TS_X,TS_Y)\neq (TG_X,TG_Y)$
</li>

<li>
$(AS_X,AS_Y)\neq (AG_X,AG_Y)$
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
$\text{case}_i$represents the $i$-th test case. Each test case is given in the following format:
</p>

<div>

$TS_X$$TS_Y$$TG_X$$TG_Y$$AS_X$$AS_Y$$AG_X$$AG_Y$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line $(1\leq i\leq T)$should contain the answer for the $i$-th test case.
</p>

<p>
Your answer will be considered correct if the absolute or relative error from the true value is at most $10^{-6}$.
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
0 0 -2 2
-1 -1 4 4
4 0 2 0
6 0 8 0
1 0 1 1
-1 0 1 1
-8 9 2 6
-10 -10 17 20

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1.000000000000000
2.000000000000000
0.000000000000000
1.783905950993199

</div>

<p>
For the first test case, let time $0$be the moment they depart. Their behavior is as follows:
</p>

<ul>

<li>
Time $0$: Takahashi departs from $(0,0)$and starts walking toward $(-2,2)$at speed $1$. At the same time, Aoki departs from $(-1,-1)$and starts walking toward $(4,4)$at speed $1$.
</li>

<li>
Time $2\sqrt{2}$: Takahashi reaches his goal point $(-2,2)$and stops. At this time, Aoki is at $(1,1)$and is still walking.
</li>

<li>
Time $5\sqrt{2}$: Aoki reaches his goal point $(4,4)$and stops.
</li>

</ul>

<p>
The distance between them is shortest at time $\frac{1}{\sqrt{2}}$, when Takahashi and Aoki are at $(-\frac{1}{2},\frac{1}{2})$and $(-\frac{1}{2},-\frac{1}{2})$respectively, and the distance is $1$.
</p>

<p>
For the second test case, the distance between them is shortest at the moment they depart, and the distance at that time is $2$.
</p>

<p>
For the third test case, the distance between them is shortest after they both stop, and the distance at that time is $0$.
</p>

</section>

</div>

</span>

</span>

</div>
