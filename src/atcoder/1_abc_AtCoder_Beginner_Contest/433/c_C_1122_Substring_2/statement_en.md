
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
You are given a string $S$consisting of digits.
</p>

<p>
A string $T$is called a 
<strong>
1122-string
</strong>
if it satisfies all of the following conditions. (The definition is the same as in Problem F.)
</p>

<ul>

<li>
$T$is a non-empty string consisting of digits.
</li>

<li>
$|T|$is even, where $|T|$denotes the length of string $T$.
</li>

<li>
All characters from the $1$-st through the $\frac{|T|}2$-th character of $T$are the same digit.
</li>

<li>
All characters from the $(\frac{|T|}2+1)$-th through the $|T|$-th character of $T$are the same digit.
</li>

<li>
Adding $1$to the digit of the $1$-st character of $T$gives the digit of the $|T|$-th character.
</li>

</ul>

<p>
For example, `1122`, `01`, and `444555`are 1122-strings, but `1222`and `90`are not 1122-strings.
</p>

<p>
Find the number of 
<strong>
substrings
</strong>
of $S$that are 1122-strings.
</p>

<p>
Two substrings are counted separately if they are extracted from different positions, even if they are identical as strings.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$S$is a string consisting of digits with length between $1$and $10^6$, inclusive.
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

$S$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the number of non-empty substrings of $S$that are 1122-strings.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

1122

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2

</div>

<p>
The following two substrings satisfy the condition.
</p>

<ul>

<li>
`12`extracted from the $2$-nd through $3$-rd characters of $S$
</li>

<li>
`1122`extracted from the $1$-st through $4$-th characters of $S$
</li>

</ul>

<p>
Thus, output $2$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

7788788

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
Note that two substrings are counted separately if they are extracted from different positions, even if they are identical as strings.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

2025

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

0

</div>

<p>
There may be no substring that is a 1122-string.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

1112222334445556555

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

11

</div>

</section>

</div>

</span>

</span>

</div>
