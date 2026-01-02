
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
You are given a triple of positive integers $(X,Y,Z)$such that $X\leq Y\leq Z$.
</p>

<p>
Output one triple of sequences of non-negative integers $(S_1,S_2,S_3)$that satisfies all of the following conditions:
</p>

<ul>

<li>
The lengths of $S_1,S_2,S_3$are each between $1$and $1000$, inclusive.
</li>

<li>
The length of a longest sequence that is both a contiguous subsequence of $S_1$and a contiguous subsequence of $S_2$is $X$.
</li>

<li>
The length of a longest sequence that is both a contiguous subsequence of $S_1$and a contiguous subsequence of $S_3$is $Y$.
</li>

<li>
The length of a longest sequence that is both a contiguous subsequence of $S_2$and a contiguous subsequence of $S_3$is $Z$.
</li>

<li>
$\max(\max(S_1),\max(S_2),\max(S_3))$is minimized among all triples satisfying the above four conditions.
</li>

</ul>

<p>
It can be proved that under the constraints of this problem, a triple $(S_1,S_2,S_3)$satisfying the conditions always exists. If there are multiple such triples, you may output any of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq X\leq Y\leq Z\leq 100$
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

$X$$Y$$Z$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output three lines.
</p>

<p>
The first line should contain $S_1$in the following format, where $|S_1|$denotes the length of $S_1$and $S_{1,i}$denotes the $i$-th element of $S_1$:
</p>

<div>

$|S_1|$$S_{1,1}$$S_{1,2}$$\dots$$S_{1,|S_1|}$
</div>

<p>
The second line should contain $S_2$and the third line should contain $S_3$, both in the same format as $S_1$.
</p>

<p>
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

4 5 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

10 1 1 0 0 1 0 1 0 1 1
8 1 1 0 1 0 0 1 1
11 1 0 0 0 1 1 0 1 0 1 0

</div>

<p>
It can be verified that $S_1=(1,1,0,0,1,0,1,0,1,1),S_2=(1,1,0,1,0,0,1,1),S_3=(1,0,0,0,1,1,0,1,0,1,0)$satisfies the conditions as follows:
</p>

<ul>

<li>
The lengths of $S_1,S_2,S_3$are $10,8,11$, respectively, all of which are between $1$and $1000$, inclusive.
</li>

<li>
The longest sequences that are both a contiguous subsequence of $S_1$and a contiguous subsequence of $S_2$are $(1,0,0,1)$and $(1,0,1,0)$, with length $X=4$.
</li>

<li>
The longest sequences that are both a contiguous subsequence of $S_1$and a contiguous subsequence of $S_3$are $(1,0,1,0,1)$and $(0,1,0,1,0)$, with length $Y=5$.
</li>

<li>
The longest sequence that is both a contiguous subsequence of $S_2$and a contiguous subsequence of $S_3$is $(1,1,0,1,0)$, with length $Z=5$.
</li>

<li>
$\max(\max(S_1),\max(S_2),\max(S_3))=1$, and it can be shown that it is impossible to satisfy the above four conditions with $\max(\max(S_1),\max(S_2),\max(S_3))=0$, so this is minimal.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
