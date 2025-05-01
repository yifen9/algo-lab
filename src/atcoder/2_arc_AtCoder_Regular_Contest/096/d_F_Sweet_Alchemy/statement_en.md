
<div>

<span>

<span>

<p>
Score : $900$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Akaki, a patissier, can make $N$kinds of doughnut using only a certain powder called "Okashi no Moto" (literally "material of pastry", simply called Moto below) as ingredient. These doughnuts are called Doughnut $1$, Doughnut $2$, $...,$Doughnut $N$. In order to make one Doughnut $i$$(1 ≤ i ≤ N)$, she needs to consume $m_i$grams of Moto. She cannot make a non-integer number of doughnuts, such as $0.5$doughnuts.
</p>

<p>
The recipes of these doughnuts are developed by repeated modifications from the recipe of Doughnut $1$. Specifically, the recipe of Doughnut $i$$(2 ≤ i ≤ N)$is a direct modification of the recipe of Doughnut $p_i$$(1 ≤ p_i < i)$.
</p>

<p>
Now, she has $X$grams of Moto. She decides to make as many doughnuts as possible for a party tonight. However, since the tastes of the guests differ, she will obey the following condition:
</p>

<ul>

<li>
Let $c_i$be the number of Doughnut $i$$(1 ≤ i ≤ N)$that she makes. For each integer $i$such that $2 ≤ i ≤ N$, $c_{p_i} ≤ c_i ≤ c_{p_i} + D$must hold. Here, $D$is a predetermined value.
</li>

</ul>

<p>
At most how many doughnuts can be made here? She does not necessarily need to consume all of her Moto.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 ≤ N ≤ 50$
</li>

<li>
$1 ≤ X ≤ 10^9$
</li>

<li>
$0 ≤ D ≤ 10^9$
</li>

<li>
$1 ≤ m_i ≤ 10^9$$(1 ≤ i ≤ N)$
</li>

<li>
$1 ≤ p_i < i$$(2 ≤ i ≤ N)$
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

$N$$X$$D$$m_1$$m_2$$p_2$$:$$m_N$$p_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the maximum number of doughnuts that can be made under the condition.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 100 1
15
10 1
20 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

7

</div>

<p>
She has $100$grams of Moto, can make three kinds of doughnuts, and the conditions that must hold are $c_1 ≤ c_2 ≤ c_1 + 1$and $c_1 ≤ c_3 ≤ c_1 + 1$. It is optimal to make two Doughnuts $1$, three Doughnuts $2$and two Doughnuts $3$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 100 10
15
10 1
20 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

10

</div>

<p>
The amount of Moto and the recipes of the doughnuts are not changed from Sample Input 1, but the last conditions are relaxed. In this case, it is optimal to make just ten Doughnuts $2$. As seen here, she does not necessarily need to make all kinds of doughnuts.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5 1000000000 1000000
123
159 1
111 1
135 3
147 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

7496296

</div>

</section>

</div>

</span>

</span>

</div>
