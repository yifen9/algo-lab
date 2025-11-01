
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given strings $A$and $B$of equal length consisting of `0`and `1`.  
</p>

<p>
You can perform the following operation on $A$zero or more times.
</p>

<ul>

<li>
Move the first character of $A$to the end.
</li>

</ul>

<p>
Find the minimum number of operations required to make $A=B$.

If it is impossible to make $A=B$no matter how you operate, print $-1$instead.
</p>

<p>
You are given $T$test cases; find the answer for each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 10000$
</li>

<li>
$A$and $B$are strings consisting of `0`and `1`.
</li>

<li>
$2 \le |A|=|B| \le 10^6$
</li>

<li>
For a single input, the sum of $|A|$does not exceed $10^6$.
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

$A$$B$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $T$lines.
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

5
1010001
1000110
000
111
01010
01010
0101
0011
100001101110000001010110110001
101100011000011011100000010101

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
-1
0
-1
22

</div>

<p>
This input contains five test cases.
</p>

<ul>

<li>
For the first test case, $A=$`1010001`and $B=$`1000110`.
<ul>

<li>
By performing the operation on $A$twice, $A$becomes `1010001`$\rightarrow$`0100011`$\rightarrow$`1000110`, which makes $A=B$.
</li>

</ul>

</li>

<li>
For the second test case, no matter how you perform the operation, you cannot change `000`to `111`.
</li>

<li>
For the third test case, $A=B$from the beginning.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
