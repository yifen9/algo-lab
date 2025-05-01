
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a monster with initial stamina $N$.

Takahashi repeatedly attacks the monster while the monster's stamina remains $1$or greater.
</p>

<p>
An attack by Takahashi reduces the monster's stamina by $2$with probability $\frac{P}{100}$and by $1$with probability $1-\frac{P}{100}$.
</p>

<p>
Find the expected value, modulo $998244353$(see Notes), of the number of attacks before the monster's stamina becomes $0$or less.  
</p>

</section>

</div>

<div>

<section>

### **Notes**

<p>
We can prove that the sought expected value is always a finite rational number.  Moreover, under the Constraints of this problem, when the value is represented as $\frac{P}{Q}$by two coprime integers $P$and $Q$, we can show that there exists a unique integer $R$such that $R \times Q \equiv P\pmod{998244353}$and $0 \leq R \lt 998244353$.  Print such $R$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 2\times 10^5$
</li>

<li>
$0 \leq P \leq 100$
</li>

<li>
All values in the input are integers.
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

$N$$P$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Find the expected value, modulo $998244353$, of the number of Takahashi's attacks.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

229596204

</div>

<p>
An attack by Takahashi reduces the monster's stamina
by $2$with probability $\frac{10}{100}=\frac{1}{10}$and by $1$with probability $\frac{100-10}{100}=\frac{9}{10}$.
</p>

<ul>

<li>
The monster's initial stamina is $3$.
</li>

<li>
After the first attack, the monster's stamina is $2$with probability $\frac{9}{10}$and $1$with probability $\frac{1}{10}$.
</li>

<li>
After the second attack, the monster's stamina is $1$with probability $\frac{81}{100}$, $0$with probability $\frac{18}{100}$, and $-1$with probability $\frac{1}{100}$.  With probability $\frac{18}{100}+\frac{1}{100}=\frac{19}{100}$, the stamina becomes $0$or less, and Takahashi stops attacking after two attacks.
</li>

<li>
If the stamina remains $1$after two attacks, the monster's stamina always becomes $0$or less by the third attack, so he stops attacking after three attacks.
</li>

</ul>

<p>
Therefore, the expected value is $2\times \frac{19}{100}+3\times\left(1-\frac{19}{100}\right)=\frac{281}{100}$.  Since $229596204 \times 100 \equiv 281\pmod{998244353}$, print $229596204$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

3

</div>

<p>
Takahashi's attack always reduces the monster's stamina by $2$.
After the second attack, the stamina remains $5-2\times 2=1$, so the third one is required.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

280 59

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

567484387

</div>

</section>

</div>

</span>

</span>

</div>
