
<div>

<span>

<span>

<div>

<section>

### **Story**

<p>
The AtCoder Kingdom is divided into an $N \times N$grid of districts, and each district has a different number of citizens.
To increase his popularity among the citizens, King Takahashi plans a tour that visits all districts exactly once by moving through districts adjacent vertically, horizontally, or diagonally.
As the tour becomes more exciting day by day, districts visited on later days yield higher favor from their residents toward Takahashi.
Please plan a tour so that the total favor Takahashi gains is as large as possible.
</p>

</section>

</div>

<div>

<section>

### **Problem Statement**

<p>
There is a kingdom divided into an $N \times N$grid of districts. Let the top-left district be $(0,0)$, and let the district reached by moving $i$districts downward and $j$districts to the right be $(i,j)$.
District $(i,j)$has $A_{i,j}$citizens.
</p>

<p>
Consider a tour that visits every district exactly once over $N^2$days, from day $0$to day $N^2-1$.
Let the district visited on day $k$be $(i_k, j_k)$.
</p>

<p>
The districts visited on two consecutive days must be adjacent 
<strong>
vertically, horizontally, or diagonally
</strong>
.
More precisely, for each $k=0,1,\dots,N^2-2$,
</p>

<p>
\[
\max\bigl(|i_k-i_{k+1}|,\ |j_k-j_{k+1}|\bigr)=1
\]
</p>

<p>
must hold.
The starting district and the ending district of the tour may be chosen arbitrarily.
</p>

<p>
For the district visited on day $k$of the tour, each resident contributes $k$favor.
The total favor Takahashi gains is
</p>

<p>
\[
\sum_{k=0}^{N^2-1} k\cdot A_{i_k, j_k}
\]
</p>

<p>
Find a visiting order that makes the total favor Takahashi gains as large as possible.
</p>

</section>

</div>

<div>

<section>

### **Scoring**

<p>
Let $V$be the total favor Takahashi gains.
Then the score for that test case is
</p>

<p>
\[
\mathrm{round}\left(\frac{V}{N^2}\right)
\]
</p>

<p>
There are $100$test cases, and the score of a submission is the total score for each test case.
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
The input is given from Standard Input in the following format.
</p>

<div>

$N$$A_{0,0}$$\cdots$$A_{0,N-1}$$\vdots$$A_{N-1,0}$$\cdots$$A_{N-1,N-1}$
</div>

<ul>

<li>
In all test cases, $N=200$.
</li>

<li>
$A_{i,j}$, the number of citizens in district $(i,j)$, is an integer satisfying $1\leq A_{i,j}\leq N^2$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $(i_k, j_k)$be the district visited on day $k$of the tour. Output to Standard Output in the following format.
</p>

<div>

$i_0$$j_0$$\vdots$$i_{N^2-1}$$j_{N^2-1}$
</div>

<p>
Your output must satisfy all of the following conditions.
</p>

<ul>

<li>
For $k=0,1,\cdots,N^2-1$, $i_k$and $j_k$are integers between $0$and $N-1$, inclusive.
</li>

<li>
All $(i_k, j_k)$for $k=0,1,\cdots,N^2-1$are distinct.
</li>

<li>
For $k=0,1,\cdots,N^2-2$, $\max(|i_k-i_{k+1}|,\ |j_k-j_{k+1}|)=1$holds.
</li>

</ul>

<p>
<a href="https://img.atcoder.jp/ahc062/u5OpcTjC.html?lang=en&seed=0&output=sample">Show example</a>
</p>

</section>

</div>

<div>

<section>

### **Input Generation**

<ul>

<li>
In all test cases, $N=200$.
</li>

<li>
The integers from $1$to $N^2$are shuffled uniformly at random, and assigned in order to $A_{0,0}, A_{0,1}, \cdots, A_{0,N-1}, A_{1,0}, \cdots, A_{N-1,N-1}$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Tools (Input generator and visualizer)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc062/u5OpcTjC.html?lang=en">Web version</a>: This is more powerful than the local version providing animations.
</li>

<li>
<a href="https://img.atcoder.jp/ahc062/u5OpcTjC.zip">Local version</a>: You need a compilation environment of <a href="https://www.rust-lang.org/">Rust language</a>.
<ul>

<li>
<a href="https://img.atcoder.jp/ahc062/u5OpcTjC_windows.zip">Pre-compiled binary for Windows</a>: If you are not familiar with the Rust language environment, please use this instead.
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
