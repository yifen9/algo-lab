
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Takahashi can combine a head part and a body part to create a robot.
A robot falls over if the weight of the head part is greater than the weight of the body part.
</p>

<p>
Currently, he has $N$head parts and $M$body parts.
The weight of the $i$-th $(1\le i\le N)$head part is $H _ i$grams, and the weight of the $i$-th $(1\le i\le M)$body part is $B _ i$grams.
</p>

<p>
He wants to create a total of $K$robots that do not fall over by appropriately combining the parts he has.
Determine whether he can achieve his goal by combining the parts well.
</p>

<p>
Here, a part cannot be used to create multiple robots, and two or more head parts (or two or more body parts) cannot be used to create one robot.
</p>

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
$1\le M\le2\times10 ^ 5$
</li>

<li>
$1\le K\le\min\lbrace N,M\rbrace$
</li>

<li>
$1\le H _ i\le10 ^ 9\ (1\le i\le N)$
</li>

<li>
$1\le B _ i\le10 ^ 9\ (1\le i\le M)$
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

$N$$M$$K$$H _ 1$$H _ 2$$\ldots$$H _ N$$B _ 1$$B _ 2$$\ldots$$B _ M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print `Yes`if Takahashi can combine the parts well to create $K$robots that do not fall over; otherwise, print `No`.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

6 6 3
2 7 1 8 2 8
1 8 2 8 4 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes

</div>

<p>
If we denote combining the $i$-th head part and the $j$-th body part as $(i,j)$, then Takahashi can create three robots that do not fall over by combining them as $(1,2),(2,4),(3,6)$, for example.
</p>

<p>
Thus, print `Yes`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1 1 1
43
1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No

</div>

<p>
His head part is too heavy, so he cannot create any robot that does not fall over.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

1 1 1
100
100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

Yes

</div>

<p>
Note that a robot does not fall over if the head and body have equal weights.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

12 15 12
748 169 586 329 972 529 432 519 408 587 138 249
656 114 632 299 984 755 404 772 155 506 832 854 353 465 387

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

Yes

</div>

</section>

</div>

</span>

</span>

</div>
