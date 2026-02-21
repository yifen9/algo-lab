
<div>

<span>

<span>

<p>
Score : $200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$customers numbered $1$to $N$, and $M$canned juices numbered $1$to $M$.
</p>

<p>
Customer $i$($1 \leq i \leq N$) has a wish list of length $L_i$. The $j$-th item ($1 \leq j \leq L_i$) from the top of customer $i$'s wish list is canned juice $X_{i,j}$. For any customer $i$, the numbers $X_{i, 1}, \dots, X_{i, L_i}$on customer $i$'s wish list are distinct.
</p>

<p>
Customers $1, \dots, N$, in this order, will now choose their beverages, following the procedure below.
</p>

<ul>

<li>
If the customer's wish list contains a canned juice that has not yet been chosen by anyone at that point, they choose the canned juice whose number appears earliest in their wish list. Otherwise, they choose water.
</li>

</ul>

<p>
Determine which beverage each customer gets.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 100$
</li>

<li>
$1 \leq M \leq 100$
</li>

<li>
$1 \leq L_i \leq M$($1 \leq i \leq N$)
</li>

<li>
$1 \leq X_{i,j} \leq M$($1 \leq i \leq N$, $1 \leq j \leq L_i$)
</li>

<li>
$X_{i, 1}, \dots, X_{i, L_i}$are distinct. ($1 \leq i \leq N$)
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

$N$$M$$L_1$$X_{1,1}$$X_{1,2}$$\cdots$$X_{1,L_1}$$L_2$$X_{2,1}$$X_{2,2}$$\cdots$$X_{2,L_2}$$\vdots$$L_N$$X_{N,1}$$X_{N,2}$$\cdots$$X_{N,L_N}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines. The $i$-th line ($1 \leq i \leq N$) should contain the number of the canned juice customer $i$gets if they get one, or `0`if customer $i$gets water.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 5
3
3 1 2
3
3 2 1
2
2 3
4
2 5 3 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
2
0
5

</div>

<p>
Among the numbers on customer $1$'s wish list, the canned juices not yet chosen by anyone are $3, 1, 2$. The one appearing earliest in the list is $3$, so customer $1$chooses canned juice $3$.
</p>

<p>
Among the numbers on customer $2$'s wish list, the canned juices not yet chosen by anyone are $2, 1$. The one appearing earliest in the list is $2$, so customer $2$chooses canned juice $2$.
</p>

<p>
For the numbers on customer $3$'s wish list, all corresponding canned juices have already been chosen by someone at that point. Thus, customer $3$chooses water.
</p>

<p>
Among the numbers on customer $4$'s wish list, the canned juices not yet chosen by anyone are $5, 1$. The one appearing earliest in the list is $5$, so customer $4$chooses canned juice $5$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6 5
1
3
2
3 5
5
5 3 1 4 2
5
5 1 3 4 2
5
3 4 1 5 2
5
5 1 3 2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

3
5
1
4
2
0

</div>

</section>

</div>

</span>

</span>

</div>
