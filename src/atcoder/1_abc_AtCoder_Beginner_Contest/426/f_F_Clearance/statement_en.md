
<div>

<span>

<span>

<p>
Score : $525$points
</p>

<div>

<section>

### **Problem Statement**

<p>
AtCoder Inc.'s online shop currently handles $N$products, and the stock of product $i$is $A_i$units remaining.  
</p>

<p>
Process the following $Q$orders in order. The $i$-th order is as follows:
</p>

<ul>

<li>
Buy $k_i$units each of products $l_i,l_i+1,\dots,r_i$. For products with fewer than $k_i$units, buy all available units. Report the total number of products bought in this order.
</li>

</ul>

<p>
Note that for $i<Q$, the stock of products bought in the $i$-th order is reduced before proceeding to the $(i+1)$-th order.
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
$1 \le N \le 3 \times 10^5$
</li>

<li>
$1 \le A_i \le 10^{15}$
</li>

<li>
$1 \le Q \le 3 \times 10^5$
</li>

<li>
$1 \le l_i \le r_i \le N$
</li>

<li>
$1 \le k_i \le 10^9$
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

$N$$A_1$$A_2$$\dots$$A_N$$Q$$l_1$$r_1$$k_1$$l_2$$r_2$$k_2$$\vdots$$l_Q$$r_Q$$k_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.

The $i$-th line should contain the total number of products bought in the $i$-th order.
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
2 6 4 5 7 5
5
1 6 1
3 5 4
4 4 1
2 5 1
1 6 100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

6
11
0
2
10

</div>

<p>
This input contains $5$orders.
</p>

<ul>

<li>
Initially, the stocks of the products are (from product $1$onward) $2,6,4,5,7,5$units.
</li>

<li>
The first order is $l_1 = 1, r_1 = 6, k_1 = 1$.
<ul>

<li>
In this order, $1,1,1,1,1,1$units of the products are bought, for a total of $6$units.
</li>

<li>
After this, the stocks of the products become $1,5,3,4,6,4$units.
</li>

</ul>

</li>

<li>
The second order is $l_2 = 3, r_2 = 5, k_2 = 4$.
<ul>

<li>
In this order, $0,0,3,4,4,0$units of the products are bought, for a total of $11$units.
</li>

<li>
After this, the stocks of the products become $1,5,0,0,2,4$units.
</li>

</ul>

</li>

<li>
The third order is $l_3 = 4, r_3 = 4, k_3 = 1$.
<ul>

<li>
In this order, $0,0,0,0,0,0$units of the products are bought, for a total of $0$units.
</li>

<li>
After this, the stocks of the products become $1,5,0,0,2,4$units.
</li>

</ul>

</li>

<li>
The fourth order is $l_4 = 2, r_4 = 5, k_4 = 1$.
<ul>

<li>
In this order, $0,1,0,0,1,0$units of the products are bought, for a total of $2$units.
</li>

<li>
After this, the stocks of the products become $1,4,0,0,1,4$units.
</li>

</ul>

</li>

<li>
The fifth order is $l_5 = 1, r_5 = 6, k_5 = 100$.
<ul>

<li>
In this order, $1,4,0,0,1,4$units of the products are bought, for a total of $10$units.
</li>

<li>
After this, the stocks of the products become $0,0,0,0,0,0$units.
</li>

</ul>

</li>

</ul>

</section>

</div>

</span>

</span>

</div>
