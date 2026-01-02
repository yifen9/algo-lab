
<div>

<span>

<span>

<p>
Score : $1100$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence $X=(X_1,X_2,\cdots,X_N)$of length $N$consisting of $0$and $1$.
</p>

<p>
You can perform the following operation zero or more times:
</p>

<ul>

<li>
Classify each element of $X$into group `A`or group `B`.
Then, for each group, reverse the order of the elements it contains.
More formally, if the elements contained in a group are $X_{i_1},X_{i_2},\cdots,X_{i_s}$($i_1<i_2<\cdots<i_s$), then for all $1 \leq j \leq s$, simultaneously replace the value of $X_{i_j}$with $X_{i_{s+1-j}}$.
</li>

</ul>

<p>
Your goal is to make $X$non-decreasing.
Find the minimum number of operations needed to achieve the goal and the way to perform the operations.
It can be proved that a solution always exists under the constraints of this problem.
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
$0 \leq X_i \leq 1$
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

$N$$X_1$$X_2$$\cdots$$X_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
For each case, output in the following format:
</p>

<div>

$k$$s_1$$s_2$$\vdots$$s_k$
</div>

<p>
Here, $k$is the minimum number of operations needed, and $s_i$is a string representing the $i$-th operation.
$s_i$is a string of length $N$consisting of `A`and `B`, and the $j$-th character of $s_i$represents the group to which $X_j$is assigned in the $i$-th operation.
If there are multiple solutions, you may output any of them.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2
4
0 1 0 1
5
0 0 1 1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
AABA
BBBB
0

</div>

<p>
For the first test case, the goal can be achieved in two operations as follows, which is the minimum number of operations:
</p>

<ul>

<li>

<p>
First operation: Use $s_1$=`AABA`. Since $(X_1,X_2,X_4)$are in group `A`, reverse their order, resulting in $(X_1,X_2,X_4)=(1,1,0)$.
Similarly, since $(X_3)$is in group `B`, reverse their order, resulting in $(X_3)=(0)$.
Thus, overall we get $X=(1,1,0,0)$.
</p>

</li>

<li>

<p>
Second operation: Use $s_2$=`BBBB`. Since $()$are in group `A`, reverse their order, resulting in $()=()$.
Similarly, since $(X_1,X_2,X_3,X_4)$are in group `B`, reverse their order, resulting in $(X_1,X_2,X_3,X_4)=(0,0,1,1)$.
Thus, overall we get $X=(0,0,1,1)$.
</p>

</li>

</ul>

<p>
For the second test case, the goal can be achieved by performing the operation zero times.
</p>

</section>

</div>

</span>

</span>

</div>
