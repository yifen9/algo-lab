
<div>

<span>

<span>

<p>
Score : $575$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given integers $N,M,K$, a length-$N$integer sequence $A=(A_0,A_1,\ldots,A_{N-1})$, and a length-$M$integer sequence $B=(B_0,B_1,\ldots,B_{M-1})$. Note that the indices start from $0$.
</p>

<p>
Find $\displaystyle\sum_{i=0}^{K-1} \min(A_{i\bmod N}, B_{i \bmod M}) $, modulo $998244353$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N,M\le 2\times 10^5$
</li>

<li>
$1\le K\le 10^{18}$
</li>

<li>
$1\le A_i,B_i\le 10^9$
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

$N$$M$$K$$A_0$$A_1$$\ldots$$A_{N-1}$$B_0$$B_1$$\ldots$$B_{M-1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $\displaystyle\sum_{i=0}^{K-1} \min(A_{i\bmod N}, B_{i \bmod M}) $, modulo $998244353$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 2 5
3 1 4
1 5

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
The desired value is $\min(3,1)+\min(1,5)+\min(4,1)+\min(3,5)+\min(1,1)=7$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 4 27
6 1 10 42
87 6 21 33

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

317

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5 7 583272014892537201
763832259 547096173 408327452 685495693 212251318
850800766 845647066 240229336 648345577 691868483 740301913 740485849

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

931208848

</div>

<p>
Compute modulo $998244353$.
</p>

</section>

</div>

</span>

</span>

</div>
