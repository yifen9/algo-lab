
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
You are given $N$strings $S_i$consisting of lowercase English letters.
</p>

<p>
For all possible permutations $P=(P_1,P_2,\dots,P_N)$of $(1,2,\dots,N)$, write down the string generated as follows:
</p>

<ul>

<li>
Concatenate $S_{P_1},S_{P_2},\dots,S_{P_N}$in this order.
</li>

</ul>

<p>
Let $A_1,A_2,\dots,A_{N!}$be the sequence of the $N!$written strings sorted in lexicographical order.

Output $A_2$.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 1.5 \times 10^5$
</li>

<li>
$2 \le N \le 3 \times 10^5$
</li>

<li>
$T,N$are integers.
</li>

<li>
$S_i$is a string consisting of lowercase English letters with length between $1$and $10^6-1$, inclusive.
</li>

<li>
For a single input, the sum of $N$does not exceed $3 \times 10^5$.
</li>

<li>
For a single input, the sum of $|S_i|$does not exceed $10^6$.
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$S_1$$S_2$$\vdots$$S_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines.
</p>

<p>
The $i$-th line should contain the answer for the $i$-th test case.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
3
abc
ac
ahc
4
aaa
a
aaaa
a
15
ks
sy
k
ysk
yks
ky
ksy
sk
syk
s
kys
sky
ys
yk
y

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

abcahcac
aaaaaaaaa
kksksykykysskskyssyksyyksykyskyys

</div>

<p>
This input contains three test cases.
</p>

<p>
For the first test case, $S=($`abc`, `ac`, `ahc`$)$.

We have $A=($`abcacahc`, `abcahcac`, `acabcahc`, `acahcabc`, `ahcabcac`, `ahcacabc`$)$, so output $A_2=$`abcahcac`.
</p>

</section>

</div>

</span>

</span>

</div>
