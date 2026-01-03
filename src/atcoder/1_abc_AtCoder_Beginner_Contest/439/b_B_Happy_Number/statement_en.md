
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
You are given a positive integer $N$. Determine whether $N$is a happy number.
</p>

<p>
A happy number is a non-negative integer that becomes $1$after repeating the following operation a finite number of times:
</p>

<ul>

<li>
Replace it with the integer obtained by taking the sum of the squares of the digits in its decimal representation.
<ul>

<li>
For example, performing this operation once on $2026$replaces it with $2^2+0^2+2^2+6^2 = 4+0+4+36 = 44$.
</li>

</ul>

</li>

</ul>

<p>
For examples of happy numbers, refer to the explanations of sample inputs and outputs.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$N$is an integer between $1$and $2026$, inclusive.
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

$N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If $N$is a happy number, output `Yes`; otherwise, output `No`.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2026

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
$2026$is a happy number.
</p>

<ul>

<li>
The digits of $2026$in decimal representation are $2,0,2,6$, and taking the sum of their squares gives $2^2+0^2+2^2+6^2 = 4+0+4+36 = 44$.
</li>

<li>
The digits of $44$in decimal representation are $4,4$, and taking the sum of their squares gives $4^2+4^2 = 16+16 = 32$.
</li>

<li>
The digits of $32$in decimal representation are $3,2$, and taking the sum of their squares gives $3^2+2^2 = 9+4 = 13$.
</li>

<li>
The digits of $13$in decimal representation are $1,3$, and taking the sum of their squares gives $1^2+3^2 = 1+9 = 10$.
</li>

<li>
The digits of $10$in decimal representation are $1,0$, and taking the sum of their squares gives $1^2+0^2 = 1+0 = 1$.
</li>

</ul>

<p>
$2026$is a happy number because it became $1$after repeating the operation of replacing itself with the integer obtained by taking the sum of the squares of the digits in its decimal representation five times.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

439

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
$439$is not a happy number.
</p>

<p>
Repeating the operation makes it $439 \rightarrow 106 \rightarrow 37 \rightarrow 58 \rightarrow 89 \rightarrow 145 \rightarrow 42 \rightarrow 20 \rightarrow 4 \rightarrow 16 \rightarrow 37 \rightarrow \dotsb$, and it can be proved that no matter how many times the operation is repeated from here, it will not become $1$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

440

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
$440$is a happy number.
</p>

</section>

</div>

</span>

</span>

</div>
