
<div>

<span>

<span>

<p>
Score : $1000$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a length-$N$positive integer sequence $A = (A_1, A_2, \ldots, A_N)$.
</p>

<p>
You are now standing at coordinate $0$on the number line, and will perform the following operation any number of times:
</p>

<ul>

<li>
Choose any element $A_i$from $A$freely. Also, choose either positive or negative direction freely.
Then, jump distance $A_i$in the chosen direction.
</li>

</ul>

<p>
You are interested in operation sequences that satisfy the following conditions:
</p>

<ul>

<li>
Perform the operation at least once and finally return to coordinate $0$.
</li>

<li>
Never enter the negative region during the process.
</li>

<li>
Never jump consecutively the same distance in different directions.
</li>

</ul>

<p>
The 
<strong>
cost
</strong>
of an operation sequence satisfying the conditions is the maximum value among the coordinates visited when moving according to that operation sequence.
Find the minimum possible cost among operation sequences satisfying the conditions.
Under the constraints of this problem, an operation sequence satisfying the conditions always exists.
</p>

<p>
Solve $T$test cases for one input.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq 125000$
</li>

<li>
$2 \leq N \leq 250000$
</li>

<li>
$1 \leq A_1 < A_2 < \cdots < A_N \leq 10^{18}$
</li>

<li>
The sum of $N$in one input does not exceed $250000$.
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

$N$$A_1$$A_2$$\cdots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
For each test case, output the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5
2
2 3
2
3 6
3
3 5 6
2
999999999999999999 1000000000000000000
3
999999999999999998 999999999999999999 1000000000000000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4
6
6
1999999999999999998
1000000000000000000

</div>

<p>
Consider the first test case.
The movement method $0 \to 2 \to 4 \to 1 \to 3 \to 0$satisfies the conditions, and the cost in this case is $4$.
There is no operation sequence with cost less than $4$, so the answer is $4$.
</p>

</section>

</div>

</span>

</span>

</div>
