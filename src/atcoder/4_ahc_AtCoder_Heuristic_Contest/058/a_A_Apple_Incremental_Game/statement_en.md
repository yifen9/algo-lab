
<div>

<span>

<span>

<div>

<section>

### **Story**

<p>
APPLE ARTIS Corporation (commonly known as AA Corporation) is a company engaged in the mass production of apples. Recently, after many years of research, they have successfully developed an innovative machine capable of generating apples from nothing.
</p>

<p>
However, to begin full-scale mass production of apples using this machine, it is necessary to mass-produce the machines themselves. To achieve this, AA Corporation has established a hierarchical system in which machines are created to produce apple-generating machines, and machines are created to produce those machine-producing machines, and so on.
</p>

<p>
As an engineer at AA Corporation, you have been tasked with developing a production planning algorithm that utilizes this hierarchy of machines to produce as many apples as possible.
</p>

</section>

</div>

<div>

<section>

### **Problem Statement**

<p>
There are $N \times L$types of machines, composed of $N$types of IDs and $L$types of Levels. A machine with Level $i$and ID $j$is referred to as 
<strong>
machine $j^i$
</strong>
($0 \leq i < L,\ 0 \leq j < N$).
</p>

<p>
The production capacity of machine $j^0$is $A_j$. The initial cost of machine $j^i$is $C_{i,j}$.
</p>

<p>
Your objective is to maximize the total number of apples at the end of $T$turns, following the procedure of the production plan below.
</p>

#### **Procedure of the Production Plan**

<p>
Let $B_{i,j}$be the number of machines $j^i$, and initially all $B_{i,j}$are set to 1.
Also, let $P_{i,j}$be the power of machine $j^i$, and initially all $P_{i,j}$are set to 0.
</p>

<p>
The initial number of apples at the start of the plan is $K$.
Each turn proceeds according to the following steps:
</p>

<ol>

<li>
You choose one of the following two actions:
<ul>

<li>
Strengthen machine $j^i$: Consume $C_{i,j} \times (P_{i,j} + 1)$apples to increase $P_{i,j}$by 1. However, you cannot strengthen if it would result in a negative number of apples.
</li>

<li>
Do nothing.
</li>

</ul>

</li>

<li>
For all machines $j^i$, perform the following in the order of Level 0, 1, 2, 3:
<ul>

<li>
For Level 0 machines ($i = 0$):
<ul>

<li>
Increase the number of apples by $A_j \times B_{i,j} \times P_{i,j}$.
</li>

</ul>

</li>

<li>
For machines of Level 1 or higher ($i \geq 1$):
<ul>

<li>
Increase $B_{i-1,j}$by $B_{i,j} \times P_{i,j}$.
</li>

</ul>

</li>

</ul>

</li>

</ol>

<p>
Choose your actions wisely to maximize the number of apples at the end of $T$turns.
</p>

</section>

</div>

<div>

<section>

### **Scoring**

<p>
Let $S$be the number of apples at the end of $T$turns. Your score is calculated as $\mathrm{round}(10^5 \times \log_2 S)$.
The higher the score, the better.
</p>

<p>
The following cases will result in a 
<span>
WA
</span>
:
</p>

<ul>

<li>
Performing a strengthening action that results in the number of apples becoming less than $0$
</li>

<li>
Specifying a non-existent machine Level or ID
</li>

<li>
Taking fewer than $T$actions
</li>

</ul>

<p>
There are $150$test cases, and the score of a submission is the total score for each test case.
If your submission produces an illegal output or exceeds the time limit for some test cases, the submission itself will be judged as 
<span>
WA
</span>
or 
<span>
TLE
</span>
, and the score of the submission will be zero.
The highest score obtained during the contest will determine the final ranking, and there will be no system test after the contest.
If more than one participant gets the same score, they will be ranked in the same place regardless of the submission time.
</p>

</section>

</div>

---

<div>

<div>

<section>

### **Input**

<p>
Input is given from Standard Input in the following format.
</p>

<div>

$N$$L$$T$$K$$A_0$$A_1$$\cdots$$A_{N-1}$$C_{0,0}$$C_{0,1}$$\cdots$$C_{0,N-1}$$C_{1,0}$$C_{1,1}$$\cdots$$C_{1,N-1}$$\vdots$$C_{L-1,0}$$C_{L-1,1}$$\cdots$$C_{L-1,N-1}$
</div>

<ul>

<li>
The first line contains four integers $N, L, T, K$:
<ul>

<li>
$N$is the number of machine IDs, and $N = 10$.
</li>

<li>
$L$is the number of machine Levels, and $L = 4$.
</li>

<li>
$T$is the total number of turns, and $T = 500$.
</li>

<li>
$K$is the number of apples at the start of the plan, and $K = 1$.
</li>

</ul>

</li>

<li>
The second line contains $N$space-separated integers $A_0, A_1, \dots, A_{N-1}$representing the production capacities of Level 0 machines:
<ul>

<li>
$A_j$is the production capacity of machine $j^0$, satisfying $1 \leq A_j \leq 100$.
</li>

<li>
$A$is sorted in ascending order ($A_0 \leq A_1 \leq \cdots \leq A_{N-1}$).
</li>

</ul>

</li>

<li>
The following $L$lines each contain $N$space-separated integers $C_{i,j}$:
<ul>

<li>
$C_{i,j}$is the initial cost of machine $j^i$, satisfying $1 \leq C_{i,j} \leq 1.25 \times 10^{12}$.
</li>

</ul>

</li>

</ul>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output exactly $T$lines.
Each line should describe the action taken on turn $t$($0 \leq t < T$), in order from turn 0, using the following format:
</p>

<ul>

<li>
To strengthen machine $j^i$:
</li>

</ul>

<div>

$i$$j$
</div>

<ul>

<li>
To do nothing:
</li>

</ul>

<div>

-1

</div>

<p>
Your program may include comment lines in the output that start with `#`.
</p>

<p>
<a href="https://img.atcoder.jp/ahc058/UpvAVdx6.html?lang=en&seed=0&output=sample">Show example</a>
</p>

</section>

</div>

<div>

<section>

### **Input Generation**

<p>
The function $\mathrm{rand\_double}(L, U)$represents generating a real number uniformly at random between $L$and $U$.
</p>

#### **Generation of $A_j$**

<ul>

<li>
When $j = 0$: set $A_0 = 1$
</li>

<li>
When $j \neq 0$: set $A_j = \mathrm{round}(10^{\mathrm{rand\_double}(0,2)})$
</li>

<li>
After generating all values, sort the array $A$in ascending order
</li>

</ul>

#### **Generation of $C_{i,j}$**

<ul>

<li>
When $i = 0$and $j = 0$: set $C_{0,0} = 1$
</li>

<li>
Otherwise: set $C_{i,j} = \mathrm{round}(A_j \times 500^i \times 10^{\mathrm{rand\_double}(0,2)})$
</li>

</ul>

</section>

</div>

<div>

<section>

### **Tools (Input generator and visualizer)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc058/UpvAVdx6.html?lang=en">Web version</a>: This is more powerful than the local version providing animations and manual play.
</li>

<li>
<a href="https://img.atcoder.jp/ahc058/UpvAVdx6.zip">Local version</a>: You need a compilation environment of <a href="https://www.rust-lang.org/">Rust language</a>.
<ul>

<li>
<a href="https://img.atcoder.jp/ahc058/UpvAVdx6_windows.zip">Pre-compiled binary for Windows</a>: If you are not familiar with the Rust language environment, please use this instead.
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
