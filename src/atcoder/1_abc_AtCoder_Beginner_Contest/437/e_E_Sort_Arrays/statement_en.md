
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
There are $N+1$sequences $A_0, A_1, \ldots, A_{N}$. $A_i$is defined as follows:
</p>

<ul>

<li>
$A_0$is an empty sequence.
</li>

<li>
$A_i\ (1\leq i\leq N)$is a sequence obtained by appending an integer $y_i$to the end of the sequence $A_{x_i}\ (0\leq x_i\lt i)$.
</li>

</ul>

<p>
Find the permutation $P=(P_1, P_2,\ldots,P_N)$of $(1,2,\ldots,N)$that satisfies the following condition:
</p>

<ul>

<li>
For $i = 1,2,\ldots,N-1$, one of the following holds:
<ul>

<li>
$A_{P_i}$is lexicographically smaller than $A_{P_{i+1}}$.
</li>

<li>
$A_{P_i}= A_{P_{i+1}}$and $P_i\lt P_{i+1}$
</li>

</ul>

</li>

</ul>

<p>
In other words, when $A_1,A_2,\ldots,A_N$are arranged in lexicographical order (when there are multiple equal sequences, arrange those with smaller indices first), $P$is the sequence of indices that appears in that arrangement.
</p>

<details>

<summary>
What is the lexicographical order of sequences?
</summary>

<p>
A sequence $S = (S_1,S_2,\ldots,S_{|S|})$is 
<strong>
lexicographically smaller
</strong>
than a sequence $T = (T_1,T_2,\ldots,T_{|T|})$if one of the following two conditions holds.
Here, $|S|$and $|T|$represent the lengths of $S$and $T$, respectively.
</p>

<ol>

<li>
$|S| \lt |T|$and $(S_1,S_2,\ldots,S_{|S|}) = (T_1,T_2,\ldots,T_{|S|})$. 
</li>

<li>
There exists an integer $1 \leq i \leq \min\lbrace |S|, |T| \rbrace$such that both of the following hold:

<ul>

<li>
$(S_1,S_2,\ldots,S_{i-1}) = (T_1,T_2,\ldots,T_{i-1})$
</li>

<li>
$S_i$is (numerically) smaller than $T_i$.
</li>

</ul>

</li>

</ol>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N\leq 3\times 10^5$
</li>

<li>
$0\leq x_i\lt i$
</li>

<li>
$1\leq y_i\leq 10^9$
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

$N$$x_1$$y_1$$x_2$$y_2$$\vdots$$x_N$$y_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $P_1, P_2, \ldots, P_N$in one line, separated by spaces.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4
0 2
0 1
2 2
0 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2 4 3 1

</div>

<p>
$A_1 = (2), A_2 = (1), A_3 = (1, 2), A_4 = (1)$, so $P=(2,4,3,1)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
0 1
0 1
0 1
0 1
0 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1 2 3 4 5

</div>

<p>
$A_1 = A_2 = A_3 = A_4 = A_5 = (1)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10
0 305186313
1 915059758
0 105282054
1 696409999
3 185928366
3 573289179
6 254538849
3 105282054
5 696409999
8 168629803

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

3 8 10 5 9 6 7 1 4 2

</div>

</section>

</div>

</span>

</span>

</div>
