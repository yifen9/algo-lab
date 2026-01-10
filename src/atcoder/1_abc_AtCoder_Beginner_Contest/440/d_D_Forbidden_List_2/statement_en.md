
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a list consisting of $N$distinct integers. The $i$-th ($1 \leq i \leq N$) integer in the list is $A_i$.
</p>

<p>
You are given $Q$questions; answer each of them. The $j$-th question ($1 \leq j \leq Q$) is as follows:
</p>

<ul>

<li>
Find the $Y_j$-th smallest value among the integers greater than or equal to $X_j$that are not in the list.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 3 \times 10^5$
</li>

<li>
$1 \leq Q \leq 3 \times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^9$($1 \leq i \leq N$)
</li>

<li>
$A_1, \dots, A_N$are distinct.
</li>

<li>
$1 \leq X_j \leq 10^9$($1 \leq j \leq Q$)
</li>

<li>
$1 \leq Y_j \leq 10^9$($1 \leq j \leq Q$)
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

$N$$Q$$A_1$$\cdots$$A_N$$X_1$$Y_1$$\vdots$$X_Q$$Y_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $j$-th line ($1 \leq j \leq Q$) should contain the answer to the $j$-th question.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 4
16 9 2 3 1
6 10
12 4
1 1
1000000000 1000000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

17
15
4
1999999999

</div>

<p>
For the first question, the smallest $10$integers greater than or equal to $6$that are not in the list are $6,\ 7,\ 8,\ 10,\ 11,\ 12,\ 13,\ 14,\ 15,\ 17$. Thus, the answer to the question is $17$.
</p>

<p>
For the second question, the smallest $4$integers greater than or equal to $12$that are not in the list are $12,\ 13,\ 14,\ 15$. Thus, the answer to the question is $15$.
</p>

<p>
For the third question, the $1$st smallest value among the integers greater than or equal to $1$that are not in the list is $4$.
</p>

<p>
For the fourth question, the $1\,000\,000\,000$-th smallest value among the integers greater than or equal to $1\,000\,000\,000$that are not in the list is $1\,999\,999\,999$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 10
284008711 658403910 982178205 50598815 694147827 230009803 763277509 509451676 821970166 284008710
740250292 159734720
255870361 8400028
23659634 718117163
697334729 301140741
698853172 270344164
713418715 285312509
50065000 52368934
46642556 591869945
607623561 273664826
482426028 265015448

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

899985013
264270388
741776803
998475472
969197337
998731226
102433934
638512505
881288390
747441478

</div>

</section>

</div>

</span>

</span>

</div>
