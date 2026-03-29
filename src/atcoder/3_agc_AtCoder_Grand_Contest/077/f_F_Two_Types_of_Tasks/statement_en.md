
<div>

<span>

<span>

<p>
Score : $1800$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$jobs numbered $1$through $N$, and you want to complete them over $N$days. You perform exactly one job per day.
</p>

<p>
Job $i$can be performed on any day from day $L_i$through day $R_i$.
Here, the following conditions are guaranteed to hold for $L_i$and $R_i$:
</p>

<ul>

<li>
$1 \leq L_i \leq i \leq R_i \leq N$
</li>

<li>
$1 \leq L_1 \leq L_2 \leq \cdots \leq L_N \leq N$
</li>

<li>
$1 \leq R_1 \leq R_2 \leq \cdots \leq R_N \leq N$
</li>

</ul>

<p>
Particularly, from the first condition, it follows that it is possible to complete all $N$jobs over $N$days.
</p>

<p>
Furthermore, each job has a type of `L`or `R`. Initially, all jobs are of type `R`.
</p>

<p>
The cost of performing a job is defined as follows:
</p>

<ul>

<li>
Suppose job $i$is performed on day $x_i$. If job $i$is of type `L`, the cost is defined as $x_i-L_i$; if it is of type `R`, the cost is defined as $R_i-x_i$.
</li>

</ul>

<p>
From now on, there will be $N$queries that change the type of a job to `L`. In the $i$-th query, the type of job $P_i$is changed to `L`.
</p>

<p>
For each $k=0,1,\ldots,N$, solve the following problem:
</p>

<ul>

<li>
Consider the state after processing the first $k$queries.
Find the minimum possible total cost of all $N$jobs.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 10^6$
</li>

<li>
$1 \leq L_i \leq i \leq R_i \leq N$
</li>

<li>
$1 \leq L_1 \leq L_2 \leq \cdots \leq L_N \leq N$
</li>

<li>
$1 \leq R_1 \leq R_2 \leq \cdots \leq R_N \leq N$
</li>

<li>
$(P_1,P_2,\ldots,P_N)$is a permutation of $(1,2,\ldots,N)$.
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

$N$$L_1$$R_1$$L_2$$R_2$$\vdots$$L_N$$R_N$$P_1$$P_2$$\ldots$$P_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
For each $k=0,1,2,\ldots,N$, output the answer in this order, separated by spaces.
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
1 3
1 3
2 3
2 1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3 1 1 2

</div>

<p>
An optimal schedule for each $k$is as follows:
</p>

<ul>

<li>
$k=0$: Perform jobs $1,2,3$on days $1,2,3$respectively. The total cost is $(3-1)+(3-2)+(3-3)=3$.
</li>

<li>
$k=1$: Perform jobs $1,2,3$on days $2,1,3$respectively. The total cost is $(3-2)+(1-1)+(3-3)=1$.
</li>

<li>
$k=2$: Perform jobs $1,2,3$on days $1,2,3$respectively. The total cost is $(1-1)+(2-1)+(3-3)=1$.
</li>

<li>
$k=3$: Perform jobs $1,2,3$on days $1,2,3$respectively. The total cost is $(1-1)+(2-1)+(3-2)=2$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4
1 4
2 4
3 4
4 4
1 2 3 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

6 3 1 0 0

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

8
1 5
1 5
2 6
2 6
3 7
3 8
5 8
5 8
5 8 7 3 2 6 4 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

17 13 10 11 7 3 6 10 14

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

15
1 4
1 4
1 8
2 8
2 11
2 11
3 11
3 11
4 12
5 12
5 13
8 14
11 15
11 15
12 15
15 13 9 3 8 11 6 5 12 2 4 7 14 1 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

44 41 37 29 22 16 12 11 16 20 21 27 35 39 42 49

</div>

</section>

</div>

</span>

</span>

</div>
