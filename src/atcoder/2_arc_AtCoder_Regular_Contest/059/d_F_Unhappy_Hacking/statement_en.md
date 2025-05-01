
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
Sig has built his own keyboard. Designed for ultimate simplicity, this keyboard only has $3$keys on it: the `0`key, the `1`key and the backspace key.
</p>

<p>
To begin with, he is using a plain text editor with this keyboard. This editor always displays one string (possibly empty). Just after the editor is launched, this string is empty. When each key on the keyboard is pressed, the following changes occur to the string:
</p>

<ul>

<li>
The `0`key: a letter `0`will be inserted to the right of the string.
</li>

<li>
The `1`key: a letter `1`will be inserted to the right of the string.
</li>

<li>
The backspace key: if the string is empty, nothing happens. Otherwise, the rightmost letter of the string is deleted.
</li>

</ul>

<p>
Sig has launched the editor, and pressed these keys $N$times in total. As a result, the editor displays a string $s$. Find the number of such ways to press the keys, modulo $10^9 + 7$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 ≦ N ≦ 5000$
</li>

<li>
$1 ≦ |s| ≦ N$
</li>

<li>
$s$consists of the letters `0`and `1`.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Partial Score**

<ul>

<li>
$400$points will be awarded for passing the test set satisfying $1 ≦ N ≦ 300$.
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

$N$$s$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the number of the ways to press the keys $N$times in total such that the editor displays the string $s$in the end, modulo $10^9+7$.
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
0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

5

</div>

<p>
We will denote the backspace key by `B`. The following $5$ways to press the keys will cause the editor to display the string `0`in the end: `00B`, `01B`, `0B0`, `1B0`, `BB0`. In the last way, nothing will happen when the backspace key is pressed.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

300
1100100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

519054663

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5000
01000001011101000100001101101111011001000110010101110010000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

500886057

</div>

</section>

</div>

</span>

</span>

</div>
