
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
Takahashi loves pepper.
</p>

<p>
A restaurant has $M$types of pepper, called type $1,2,\dots,M$. There are $C_j$grams of type $j$($1 \le j \le M$) pepper at this restaurant.  
</p>

<p>
He ordered $N$dishes at this restaurant.

Due to compatibility, only type $A_i$pepper can be sprinkled on dish $i$($1 \le i \le N$), and the upper limit on the amount of pepper that can be sprinkled on dish $i$is $B_i$grams.

Also, he can only use the pepper available at the restaurant. That is, the total amount of type $j$pepper sprinkled cannot exceed $C_j$grams.
</p>

<p>
He decides how much pepper to sprinkle on each dish to maximize the total amount of pepper sprinkled on the dishes.

How many grams of pepper in total can he sprinkle on the dishes?
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
$1 \le N,M \le 1000$
</li>

<li>
$1 \le A_i \le M$
</li>

<li>
$1 \le B_i,C_i \le 10^6$
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

$N$$M$$C_1$$C_2$$\dots$$C_M$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_N$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer as an integer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

7 5
4 4 8 3 7
1 2
2 3
5 2
4 10
2 3
5 4
2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

15

</div>

<p>
In this input, there are five types of pepper, with $4,4,8,3,7$grams of type $1,2,3,4,5$pepper respectively.

The following gives a total of $15$grams of pepper sprinkled on the dishes, which is the maximum achievable.
</p>

<ul>

<li>
Sprinkle $2$grams of type $1$pepper on dish $1$.
</li>

<li>
Sprinkle no pepper on dish $2$.
</li>

<li>
Sprinkle $2$grams of type $5$pepper on dish $3$.
</li>

<li>
Sprinkle $3$grams of type $4$pepper on dish $4$.
</li>

<li>
Sprinkle $1$gram of type $2$pepper on dish $5$.
</li>

<li>
Sprinkle $4$grams of type $5$pepper on dish $6$.
</li>

<li>
Sprinkle $3$grams of type $2$pepper on dish $7$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1 1
1
1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

15 10
7 94 100 82 63 81 75 2 76 73
10 44
5 77
10 47
7 32
2 82
5 90
3 37
6 70
6 28
3 25
2 26
10 56
1 69
5 46
7 26

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

438

</div>

</section>

</div>

</span>

</span>

</div>
