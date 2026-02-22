
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$people with distinct surnames, and the surname of the $i$-th person has parameters $(X_i, Y_i, Z_i)$. Different surnames may have identical parameters.
The following event occurs $N - 1$times.
</p>

<ul>

<li>
Two people become parents and one child appears. The two parents die. The child chooses the stronger of the two parents' surnames as their own. A surname with parameters $(x_1, y_1, z_1)$is stronger than a surname with parameters $(x_2, y_2, z_2)$if $x_1 > x_2$, $y_1 > y_2$, and $z_1 > z_2$all hold. If neither parent's surname is stronger than the other's, the child randomly chooses one of the two parents' surnames.
</li>

</ul>

<p>
Find the number of people among the $N$people whose surname can be the surname of the last remaining person.
</p>

<p>
You are given $T$test cases; solve each one.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 2 \times 10^5$
</li>

<li>
$2 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le X_i, Y_i, Z_i \le N$
</li>

<li>
The sum of $N$over all test cases is at most $2 \times 10^5$.
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
Each test case is given in the following format:
</p>

<div>

$N$$X_1$$Y_1$$Z_1$$X_2$$Y_2$$Z_2$$\vdots$$X_N$$Y_N$$Z_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines.
</p>

<p>
The $i$-th line should contain the number of people whose surname can be the surname of the last remaining person for the $i$-th test case.
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
4
3 4 4
2 2 2
4 3 3
1 1 1
3
2 1 1
1 2 1
1 1 2
3
2 2 2
2 2 2
1 1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
3
2

</div>

<p>
For the first test case, below is a possible sequence of events.
</p>

<p>
Let surname $i$denote the surname of the $i$-th person.
</p>

<ul>

<li>
The people with surnames $2$and $4$become parents. Surname $2$is stronger, so the child has surname $2$.
</li>

<li>
The people with surnames $2$and $3$become parents. Surname $3$is stronger, so the child has surname $3$.
</li>

<li>
The people with surnames $1$and $3$become parents. Neither surname $1$nor surname $3$is stronger than the other, so the child chooses either surname $1$or $3$.
</li>

</ul>

<p>
Neither surname $2$nor surname $4$can be the surname of the last remaining person, so the answer is $2$.
</p>

</section>

</div>

</span>

</span>

</div>
