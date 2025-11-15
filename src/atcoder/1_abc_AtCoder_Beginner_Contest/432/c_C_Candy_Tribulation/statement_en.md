
<div>

<span>

<span>

<p>
Score : $350$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You have an unlimited supply of two types of candies: small candies and large candies.
The weight of a small candy is $X$grams, and the weight of a large candy is $Y$grams. Large candies are heavier than small candies (that is, $X < Y$).
</p>

<p>
There are $N$children, numbered $1$to $N$.
</p>

<p>
You have decided to distribute candies so that the following conditions are satisfied:
</p>

<ul>

<li>
For $i=1,\dots,N$, child $i$receives exactly $A_i$candies in total of the two types.
</li>

<li>
The total weights of candies distributed to the $N$children are all equal.
</li>

</ul>

<p>
Determine whether there exists a distribution method that satisfies the conditions. If it exists, find the maximum possible value for the number of large candies distributed.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^9$
</li>

<li>
$1 \leq X < Y \leq 10^9$
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

$N$$X$$Y$$A_1$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If there is no distribution method that satisfies the conditions, output `-1`.
</p>

<p>
If there exists a distribution method that satisfies the conditions, output the maximum possible value for the number of large candies distributed in such a distribution method.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 6 8
11 10 13

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

18

</div>

<p>
You can distribute candies as follows so that the total weights of candies distributed to the children are all equal.
</p>

<ul>

<li>
Child $1$receives $4$small candies and $7$large candies. The total weight is $6 \times 4 + 8 \times 7 = 80$grams.
</li>

<li>
Child $2$receives $0$small candies and $10$large candies. The total weight is $6 \times 0 + 8 \times 10 = 80$grams.
</li>

<li>
Child $3$receives $12$small candies and $1$large candy. The total weight is $6 \times 12 + 8 \times 1 = 80$grams.
</li>

</ul>

<p>
In this distribution method, a total of $18$large candies are distributed.
</p>

<p>
There is no distribution method that satisfies the conditions and distributes more than $18$large candies. Therefore, the answer is $18$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2 3 4
3 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1

</div>

<p>
There is no distribution method that satisfies the conditions.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

8 4 32
1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

8000000000

</div>

<p>
The answer may not fit in a 32-bit integer.
</p>

</section>

</div>

</span>

</span>

</div>
