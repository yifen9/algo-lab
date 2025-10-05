
<div>

<span>

<span>

<p>
Score : $800$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence of length $N$, $A=(A_1, A_2, \cdots, A_N)$.
Snuke wants to make $A$a non-decreasing sequence.
</p>

<p>
He can perform the following operation zero or more times.
</p>

<ul>

<li>
Choose two adjacent elements of $A$
</li>

<li>
Remove these two elements and insert the bitwise $\mathrm{OR}$of these two values at the original position
</li>

</ul>

<p>
Find the maximum possible value of the length of $A$when $A$becomes a non-decreasing sequence.
</p>

<details>

<summary>
What is bitwise $\mathrm{OR}$?
  
</summary>

<p>
The bitwise $\mathrm{OR}$of non-negative integers $A$and $B$, $A\ \mathrm{OR}\ B$, is defined as follows.
    
</p>

<ul>

<li>
When $A\ \mathrm{OR}\ B$is written in binary, the digit in the $2^k$place ($k \geq 0$) is $1$if at least one of the digits in the $2^k$place of $A$and $B$written in binary is $1$, and $0$otherwise.
</li>

</ul>
For example, $3\ \mathrm{OR}\ 5 = 7$(in binary: $011\ \mathrm{OR}\ 101 = 111$).
  
<p>

</p>

</details>

<details>

<summary>
What is a non-decreasing sequence?
  
</summary>

<p>
A sequence $a=(a_1,a_2, \cdots, a_n)$is a non-decreasing sequence if and only if $a_1 \le a_2 \le \ldots \le a_n$holds.
  
</p>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le A_i <2^{30}$
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

$N$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answer.
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
3 1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2

</div>

<ul>

<li>
If the $1$-st and $2$-nd elements are chosen in the first operation, $A=(3,2)$and $A$is not a non-decreasing sequence.
</li>

<li>
If the $2$-nd and $3$-rd elements are chosen in the first operation, $A=(3,3)$and $A$is a non-decreasing sequence.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4
4 1 2 3

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

20
105327673 847116534 928167271 478716741 244808645 744985167 772409400 950055714 32441819 24475691 74630537 632066724 170250355 937572655 791196964 469960355 264764288 1061830134 183233398 643628719

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

7

</div>

</section>

</div>

</span>

</span>

</div>
