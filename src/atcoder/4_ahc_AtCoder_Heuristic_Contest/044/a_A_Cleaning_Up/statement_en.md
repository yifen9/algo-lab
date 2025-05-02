
<div>

<span>

<span>

<div>

<section>

### **Story**

<p>
A company is currently aiming to create a comfortable working environment. It has decided to clean the office every week starting this April, when new employees join the company.
However, assigning cleaning duties is not easy. There are various constraints, for example, the duty should not be concentrated on one person, and the burden on new employees, who are not yet accustomed to the work, should be especially low.
Also, the assignment should be easy to remember, like "after employee X, the next must be employee Y or Z."
Create a cleaning plan that follows the constraints as closely as possible.
</p>

</section>

</div>

<div>

<section>

### **Problem Statement**

<p>
There are $N$employees in a company, numbered from $0$to $N-1$.
For each employee $i$$(0 \leq i \leq N-1)$, you must determine two integers $a_i$and $b_i$($a_i$and $b_i$may be equal).
Then, the cleaning plan for each week is created in the following way:
</p>

<ul>

<li>
In the first week, employee $0$will do the cleaning.
</li>

<li>
From the second week onward, let employee $x$be the one who did the cleaning last week, and let $t$be the number of weeks in which employee $x$had been assigned as the cleaner by the end of last week. Then, this week's cleaning duty is determined as follows:
<ul>

<li>
When $t$is odd: employee $a_x$
</li>

<li>
When $t$is even: employee $b_x$
</li>

</ul>

</li>

</ul>

<p>
For each $i$$(0 \leq i \leq N-1)$, a target number of times $T_i$is given as the number of times employee $i$should be assigned cleaning duty in the next $L = 500\,000$weeks.
Let $t_i$be the actual number of times employee $i$is assigned cleaning duty.
Create a cleaning plan that makes the error defined by $\left|t_0 - T_0\right| + \left|t_1 - T_1\right| + \cdots + \left|t_{N-1} - T_{N-1}\right|$as small as possible.
</p>

</section>

</div>

<div>

<section>

### **Scoring**

<p>
Let $E$be the error in the output cleaning plan. You will obtain the score of $10^6 - E$, which is guaranteed to be non-negative.
</p>

<p>
There are 150 testcases, and the score of a submission is the total score for each testcase. If your submission produces an illegal output or exceeds the time limit for some testcases, the submission itself will be judged as 
<span>
WA
</span>
or 
<span>
TLE
</span>
, and the score of the submission will be zero. The highest score obtained during the contest will determine the final ranking, and there will be no system test after the contest. If more than one participant gets the same score, they will be ranked in the same place regardless of the submission time.
</p>

</section>

</div>

---

<div>

<div>

<section>

### **Input**

<p>
Input is given from Standard Input in the following format:
</p>

<div>

$N$$L$$T_0$$T_1$$\cdots$$T_{N-1}$
</div>

<ul>

<li>
The number of employees $N$is fixed to $100$across all testcases.
</li>

<li>
The number of weeks $L$is fixed to $500\,000$across all testcases.
</li>

<li>
$0 \leq T_i \leq 10\,000$.
</li>

<li>
$T_0 + T_1 + \cdots + T_{N-1} = L$.
</li>

<li>
Given values are all integers.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output to Standard Output in the following format:
</p>

<div>

$a_0$$b_0$$a_1$$b_1$$\vdots$$a_{N-1}$$b_{N-1}$
</div>

<p>
Here, if there exists an $i$$(0 \leq i \leq N-1)$that does not satisfy $0 \leq a_i \leq N-1$or $0 \leq b_i \leq N-1$, the output will be judged as 
<span>
WA
</span>
.
</p>

<p>
<a href="https://img.atcoder.jp/ahc044/PnJFT8lu.html?lang=en&seed=0&output=sample">Show example</a>
</p>

</section>

</div>

<div>

<section>

### **Input Generation**

<p>
Let $\mathrm{rand}(L, U)$be the function that generates a uniform random integer between $L$and $U$, inclusive. The input will be generated in the following algorithm:
</p>

<ol>

<li>
For each $i$$(0 \leq i \leq N-2)$, generate $T_i$with $\mathrm{rand}(0, 10000)$.
</li>

<li>
If the sum $S = T_0 + \cdots + T_{N-2}$satisfies $0 \leq L - S \leq 10000$, set $T_{N-1} = L - S$and finalize the input. Otherwise, retry step 1.
</li>

</ol>

</section>

</div>

<div>

<section>

### **Tools (Input generator and visualizer)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc044/PnJFT8lu.html?lang=en">Web version</a>: This is more powerful than the local version providing animations.
</li>

<li>
<a href="https://img.atcoder.jp/ahc044/PnJFT8lu.zip">Local version</a>: You need a compilation environment of <a href="https://www.rust-lang.org/">Rust language</a>.
<ul>

<li>
<a href="https://img.atcoder.jp/ahc044/PnJFT8lu_windows.zip">Pre-compiled binary for Windows</a>: If you are not familiar with the Rust language environment, please use this instead.
</li>

</ul>

</li>

</ul>

<p>
Please be aware that sharing visualization results or discussing solutions/ideas during the contest is prohibited.
</p>

</section>

</div>

</div>

</span>

</span>

</div>
