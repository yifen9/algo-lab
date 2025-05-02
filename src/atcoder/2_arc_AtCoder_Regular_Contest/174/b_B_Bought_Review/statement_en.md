
<div>

<span>

<span>

<p>
Score: $300$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Solve the following problem for $T$test cases.
</p>

<p>
On the gourmet review site EatCocoder, you can review restaurants with an integer number of stars from $1$to $5$.

Initially, the restaurant managed by Chef B has $A_i$reviews with $i$stars. $(1 \le i \le 5)$

The chef can pay a bribe of $P_i$yen to the EatCocoder administration to have one additional $i$-star review. $(1 \le i \le 5)$
</p>

<p>
After adding a total of $k$reviews by bribery, there will be $A_1+A_2+A_3+A_4+A_5+k$reviews in total.

Chef B wants the average rating of these reviews to be at least $3$stars. Determine the minimum total amount of bribery required to achieve this.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
All input values are integers.
</li>

<li>
$1 \le T \le 10^4$
</li>

<li>
$0 \le A_i \le 10^8$
</li>

<li>
$1 \le A_1+A_2+A_3+A_4+A_5$
</li>

<li>
$1 \le P_i \le 10^8$
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

$T$$\rm{Case}_1$$\rm{Case}_2$$\vdots$$\rm{Case}$$_T$
</div>

<p>
Here, $\rm{Case}$$_i$represents the $i$-th test case.

Each test case is given in the following format:
</p>

<div>

$A_1$$A_2$$A_3$$A_4$$A_5$$P_1$$P_2$$P_3$$P_4$$P_5$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $T$lines in total.

The $i$-th line should contain the answer to the $i$-th test case as an integer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

6
1 0 1 0 0
1 2 3 4 5
0 2 2 0 0
1 1 1 1 5
0 1 2 0 0
1 1 1 5 3
1 1 1 0 0
1 1 1 1 1
0 0 0 0 1
1 1 1 1 1
100000000 100000000 100000000 0 0
100000000 100000000 100000000 100000000 100000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

5
2
3
2
0
15000000000000000

</div>

<p>
This input contains six test cases.
</p>

<ul>

<li>
For the first test case, you can, for example, do the following to have an average rating of at least $3$stars with a bribe of $5$yen, which is the minimum possible amount.
<ul>

<li>
Initially, there are $1,0,1,0,0$reviews with $1,2,3,4,5$stars, respectively.
</li>

<li>
Pay a bribe of $P_5 = 5$yen to add one $5$-star review.
</li>

<li>
As a result, there are $1,0,1,0,1$reviews with $1,2,3,4,5$stars, respectively, averaging $3$stars.
</li>

</ul>

</li>

<li>
For the second test case, you can, for example, do the following to have an average rating of at least $3$stars with a bribe of $2$yen, which is the minimum possible amount.
<ul>

<li>
Initially, there are $0,2,2,0,0$reviews with $1,2,3,4,5$stars, respectively.
</li>

<li>
Pay a bribe of $P_4 \times 2 = 2$yen to add two $4$-star reviews.
</li>

<li>
As a result, there are $0,2,2,2,0$reviews of with $1,2,3,4,5$stars, respectively, averaging $3$stars.
</li>

</ul>

</li>

<li>
For the third test case, you can, for example, do the following to have an average rating of at least $3$stars with a bribe of $3$yen, which is the minimum possible amount.
<ul>

<li>
Initially, there are $0,1,2,0,0$reviews with $1,2,3,4,5$stars, respectively.
</li>

<li>
Pay a bribe of $P_5 = 3$yen to add one $5$-star review.
</li>

<li>
As a result, there are $0,1,2,0,1$reviews with $1,2,3,4,5$stars, respectively, averaging $3.25$stars.
</li>

</ul>

</li>

<li>
For the fourth test case, you can, for example, do the following to have an average rating of at least $3$stars with a bribe of $2$yen, which is the minimum possible amount.
<ul>

<li>
Initially, there are $1,1,1,0,0$reviews with $1,2,3,4,5$stars, respectively.
</li>

<li>
Pay a bribe of $P_4 = 1$yen to add one $4$-star review.
</li>

<li>
Pay a bribe of $P_5 = 1$yen to add one $5$-star review.
</li>

<li>
As a result, there are $1,1,1,1,1$reviews with $1,2,3,4,5$stars, respectively, averaging $3$stars.
</li>

</ul>

</li>

<li>
For the fifth test case, you can, for example, do the following to have an average rating of at least $3$stars with a bribe of $0$yen, which is the minimum possible amount.
<ul>

<li>
Initially, there are $0,0,0,0,1$reviews with $1,2,3,4,5$stars, respectively.
</li>

<li>
Since the average is already $5$, which is not less than $3$, give no bribe.
</li>

</ul>

</li>

<li>
For the sixth test case, note that the answer may not fit into a $32$-bit signed integer.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
