
<div>
﻿
<span>

<span>

<p>
Score : $625$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Takahashi will receive some presents from now on.
</p>

<p>
He has an integer parameter called mood, and the mood changes each time he receives a present.
Each present has an integer parameter called value $P$, and Takahashi's mood changes according to this parameter as follows:
</p>

<ul>

<li>
If the value $P$of the received present is greater than or equal to the mood value, he is delighted with the present, and the mood increases by $A$.
</li>

<li>
If the value $P$of the received present is less than the mood value, he is disappointed with the present, and the mood decreases by $B$.
</li>

</ul>

<p>
Initially, there are $N$presents that Takahashi is scheduled to receive, and the value of the $i$-th present he will receive $(1\le i\le N)$is $P _ i$.
</p>

<p>
You are given $Q$queries consisting of two types: addition queries and question queries. Process all of them in order, and answer all question queries.
</p>

<p>
The $i$-th query is represented by two integers $T _ i,X _ i$, and it is an addition query if $T _ i=1$, and a question query if $T _ i=2$.
</p>

<p>
In an addition query, add a new present with value $X _ i$to the end of the presents to be received.
</p>

<p>
In a question query, answer the following question:
</p>

<blockquote>

<p>
Find Takahashi's mood after receiving all the presents he is scheduled to receive when his mood is initially $X _ i$.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le2\times10 ^ 5$
</li>

<li>
$1\le A\le10 ^ 9$
</li>

<li>
$1\le B\le10 ^ 9$
</li>

<li>
$-10 ^ 9\le P _ i\le10 ^ 9\ (1\le i\le N)$
</li>

<li>
$1\le Q\le2\times10 ^ 5$
</li>

<li>
$T _ i=1$or $T _ i=2\ (1\le i\le Q)$
</li>

<li>
There exists an integer $i\ (1\le i\le Q)$such that $T _ i=2$.
</li>

<li>
If $T _ i=1$, then $-10 ^ 9\le X _ i\le10 ^ 9$. $(1\le i\le Q)$
</li>

<li>
If $T _ i=2$, then $-10 ^ {12}\le X _ i\le10 ^ {12}$. $(1\le i\le Q)$
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

$N$$A$$B$$P _ 1$$P _ 2$$\ldots$$P _ N$$Q$$T _ 1$$X _ 1$$T _ 2$$X _ 2$$\vdots$$T _ Q$$X _ Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $q$be the number of question queries, and print $q$lines.
The $i$-th line $(1\le i\le q)$should contain the answer to the $i$-th question query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 31 41
59 -26 53 58
5
2 9
1 79
2 32
1 38
2 462

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

61
43
216

</div>

<p>
Initially, the values of the presents Takahashi is scheduled to receive are $59,-26,53,58$, in the order he will receive them.
</p>

<p>
The five queries are as follows:
</p>

<ul>

<li>
When his mood is initially $9$, his mood changes as $9\rightarrow40\rightarrow-1\rightarrow30\rightarrow61$each time he receives a present, so print the final mood $61$.
</li>

<li>
A present with value $79$is added to the presents he is scheduled to receive, and the values of the presents he is scheduled to receive become $59,-26,53,58,79$.
</li>

<li>
When his mood is initially $32$, his mood changes as $32\rightarrow63\rightarrow22\rightarrow53\rightarrow84\rightarrow43$each time he receives a present, so print the final mood $43$.
</li>

<li>
A present with value $38$is added to the presents he is scheduled to receive, and the values of the presents he is scheduled to receive become $59,-26,53,58,79,38$.
</li>

<li>
When his mood is initially $462$, his mood changes as $462\rightarrow421\rightarrow380\rightarrow339\rightarrow298\rightarrow257\rightarrow216$each time he receives a present, so print the final mood $216$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 1000000000 1000000000
1000000000 0 -1000000000
3
2 -1000000000000
2 0
2 1000000000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-997000000000
-1000000000
997000000000

</div>

<p>
Note that the absolute value of the input and the values to be output may be $2 ^ {32}$or greater.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

20 8489 1428
6312 -9511 1048 -5301 -2588 -7097 -3342 5209 7493 3378 -5300 6592 7862 -8118 8109 1116 5549 3953 9244 7773
10
1 1694
2 -9723
2 -5195
2 -1384
1 1149
2 9845
2 -7720
2 8329
2 -4652
2 -5672

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

9874
14402
8296
8180
10449
6664
3600
12497

</div>

</section>

</div>

</span>

</span>

</div>
