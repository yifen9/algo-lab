
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
You have $N$bamboos. The lengths (in centimeters) of these are $l_1, l_2, ..., l_N$, respectively.
</p>

<p>
Your objective is to use some of these bamboos (possibly all) to obtain three bamboos of length $A, B, C$. For that, you can use the following three kinds of magics any number:
</p>

<ul>

<li>
Extension Magic: Consumes $1$
<em>
MP
</em>
(magic point). Choose one bamboo and increase its length by $1$.
</li>

<li>
Shortening Magic: Consumes $1$MP. Choose one bamboo of length at least $2$and decrease its length by $1$.
</li>

<li>
Composition Magic: Consumes $10$MP. Choose two bamboos and combine them into one bamboo. The length of this new bamboo is equal to the sum of the lengths of the two bamboos combined. (Afterwards, further magics can be used on this bamboo.)
</li>

</ul>

<p>
At least how much MP is needed to achieve the objective?
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3 \leq N \leq 8$
</li>

<li>
$1 \leq C < B < A \leq 1000$
</li>

<li>
$1 \leq l_i \leq 1000$
</li>

<li>
All values in input are integers.
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
Input is given from Standard Input in the following format:
</p>

<div>

$N$$A$$B$$C$$l_1$$l_2$$:$$l_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the minimum amount of MP needed to achieve the objective.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 100 90 80
98
40
30
21
80

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

23

</div>

<p>
We are obtaining three bamboos of lengths $100, 90, 80$from five bamboos $98, 40, 30, 21, 80$. We already have a bamboo of length $80$, and we can obtain bamboos of lengths $100, 90$by using the magics as follows at the total cost of $23$MP, which is optimal.
</p>

<ol>

<li>
Use Extension Magic twice on the bamboo of length $98$to obtain a bamboo of length $100$. (MP consumed: $2$)
</li>

<li>
Use Composition Magic on the bamboos of lengths $40, 30$to obtain a bamboo of length $70$. (MP consumed: $10$)
</li>

<li>
Use Shortening Magic once on the bamboo of length $21$to obtain a bamboo of length $20$. (MP consumed: $1$)
</li>

<li>
Use Composition Magic on the bamboo of length $70$obtained in step 2 and the bamboo of length $20$obtained in step 3 to obtain a bamboo of length $90$. (MP consumed: $10$)
</li>

</ol>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

8 100 90 80
100
100
90
90
90
80
80
80

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

<p>
If we already have all bamboos of the desired lengths, the amount of MP needed is $0$. As seen here, we do not necessarily need to use all the bamboos.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

8 1000 800 100
300
333
400
444
500
555
600
666

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

243

</div>

</section>

</div>

</span>

</span>

</div>
