
<div>

<span>

<span>

<p>
Score : $550$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<p>
At AtCoder Ranch, horses bathe themselves. Some horses clean up afterward, while others leave a mess.
</p>

</blockquote>

<p>
There are $N$horses, numbered $1$to $N$. Horse $i$($1 \leq i \leq N$) has a 
<strong>
mood
</strong>
$A_i$and a 
<strong>
tidiness
</strong>
$B_i$(where $B_i$is $1$or $2$).
</p>

<p>
At night, the $N$horses bathe once each. Let $p_j$be the number of the horse that bathes in the $j$-th turn ($1 \leq j \leq N$). The 
<strong>
satisfaction
</strong>
of horse $p_j$is given as follows:
</p>

<ul>

<li>
If $j \geq 2$, the product of the mood of horse $p_j$and the tidiness of horse $p_{j-1}$.
</li>

<li>
If $j = 1$, the mood of horse $p_j$.
</li>

</ul>

<p>
You will be given $Q$queries, one for each day over $Q$days. Process them in order. The query for the $k$-th day ($1 \leq k \leq Q$) is as follows:
</p>

<ul>

<li>
Change the mood of horse $W_k$to $X_k$and its tidiness to $Y_k$(where $Y_k$is $1$or $2$). Then, find the maximum possible total satisfaction of the $N$horses' baths that night if you can decide the order in which the $N$horses bathe arbitrarily.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq Q \leq 2 \times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^6$($1 \leq i \leq N$)
</li>

<li>
$B_i$is $1$or $2$. ($1 \leq i \leq N$)
</li>

<li>
$1 \leq W_k \leq N$($1 \leq k \leq Q$)
</li>

<li>
$1 \leq X_k \leq 10^6$($1 \leq k \leq Q$)
</li>

<li>
$Y_k$is $1$or $2$. ($1 \leq k \leq Q$)
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

$N$$Q$$A_1$$B_1$$\vdots$$A_N$$B_N$$W_1$$X_1$$Y_1$$\vdots$$W_Q$$X_Q$$Y_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $k$-th line ($1 \leq k \leq Q$) should contain the answer to the query for the $k$-th day.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 4
1 2
10 1
3 1
7 2
2 7 1
1 3 1
2 2 1
3 1000000 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

32
27
18
2000015

</div>

<p>
For the query on the first day, if the horses bathe in the order $3,1,4,2$, the satisfaction of each horse is as follows:
</p>

<ul>

<li>
Horse $3$'s satisfaction is $3$
</li>

<li>
Horse $1$'s satisfaction is $1 \times 1 = 1$
</li>

<li>
Horse $4$'s satisfaction is $7 \times 2 = 14$
</li>

<li>
Horse $2$'s satisfaction is $7 \times 2 = 14$
</li>

</ul>

<p>
The total satisfaction in this case is $32$.
</p>

<p>
For the query on the second day, if the horses bathe in the order $4,2,1,3$, the satisfaction of each horse is as follows:
</p>

<ul>

<li>
Horse $4$'s satisfaction is $7$
</li>

<li>
Horse $2$'s satisfaction is $7 \times 2 = 14$
</li>

<li>
Horse $1$'s satisfaction is $3 \times 1 = 3$
</li>

<li>
Horse $3$'s satisfaction is $3 \times 1 = 3$
</li>

</ul>

<p>
The total satisfaction in this case is $27$.
</p>

<p>
For the query on the third day, if the horses bathe in the order $4,3,2,1$, the total satisfaction is $18$.
</p>

<p>
For the query on the fourth day, if the horses bathe in the order $4,3,1,2$, the total satisfaction is $2000015$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 10
340019 2
598908 1
177330 2
575439 2
916653 2
451275 2
762769 2
36625 2
273231 2
367619 2
8 334230 2
8 835378 1
4 777076 2
6 61501 1
4 516395 1
4 35678 2
5 751493 1
3 815798 1
2 369777 2
5 941470 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

9417616
10146681
10549955
9708906
8847525
8463663
7860112
8606740
8516097
9236070

</div>

</section>

</div>

</span>

</span>

</div>
