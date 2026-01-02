
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
There is a traffic signal. This signal is always red, but when PCT-kun pays $P$yen and presses a button, it becomes green for $X$seconds. However, he must follow the following rules:
</p>

<ul>

<li>
The button can only be pressed at timings that can be expressed as time $t$for an integer $t$. (Negative integers can also be chosen as $t$.)
</li>

<li>
If the button is pressed at time $t$, it cannot be pressed until time $t+Y$. (It can be pressed at time $t+Y$.)
</li>

</ul>

<p>
There are $N$people crossing this signal. The $i$-th person tries to cross this signal at time $A_i + 0.5$, and if the signal is green at time $A_i + 0.5$, they pay $C_i$yen to PCT-kun.
</p>

<p>
Find the maximum possible value of money received by PCT-kun minus the cost of pressing the button.
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
$1 \le T \le 2 \times 10^5$
</li>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le P \le 10^9$
</li>

<li>
$1 \le X \le Y \le 10^9$
</li>

<li>
$1 \le A_i \le 10^{18}$
</li>

<li>
$1 \le C_i \le 10^9$
</li>

<li>
The sum of $N$over all test cases is at most $2 \times 10^5$.
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each case is given in the following format:
</p>

<div>

$N$$P$$X$$Y$$A_1$$A_2$$\dots$$A_N$$C_1$$C_2$$\dots$$C_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line $(1 \le i \le T)$should contain the answer for $\mathrm{case}_i$.
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
3 4 5 12
3 5 11
6 2 9
4 2 1 1
1 2 3 4
100 100 100 1
7 37 21 41
80 136 88 102 161 91 115
61 1 11 86 17 59 91
10 2763 2591 3369
2735 7773 36286 43737 9840 21707 19921 45759 44170 45287
3287 8050 3485 6845 3784 4565 3345 9297 2010 5550
15 408094769 859747485 886452311
1760053960 6327322912 490407029 1899495636 1174752626 84645660 6211206638 270040559 6098433044 4316510828 6601842919 5644655565 243073507 3150320792 4408022586
872391155 333542193 911310678 545186339 707811244 197915352 984885281 162966691 939525712 161385193 129092590 700676660 546046296 128723014 931663769

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

7
294
164
36403
6362927487

</div>

<p>
For the first test case, here is an example of PCT-kun's actions:
</p>

<ul>

<li>
Pay $4$yen and press the button at time $-1$. This makes the signal green from time $-1$to time $4$.
</li>

<li>
Person $1$comes at time $3.5$. Since the signal is green, they pay $6$yen to him.
</li>

<li>
Person $2$comes at time $5.5$. Since the signal is red, nothing happens.
</li>

<li>
Pay $4$yen and press the button at time $11$. This makes the signal green from time $11$to time $16$.
</li>

<li>
Person $3$comes at time $11.5$. Since the signal is green, they pay $9$yen to him.
</li>

</ul>

<p>
In this case, the money received by him minus the cost of pressing the button is $7$yen, and it can be proved that $7$yen is the maximum value.
</p>

<p>
For the second test case, here is an example of his actions:
</p>

<ul>

<li>
Pay $2$yen and press the button at time $1$. This makes the signal green from time $1$to time $2$.
</li>

<li>
Person $1$comes at time $1.5$. Since the signal is green, they pay $100$yen to him.
</li>

<li>
Pay $2$yen and press the button at time $2$. This makes the signal green from time $2$to time $3$.
</li>

<li>
Person $2$comes at time $2.5$. Since the signal is green, they pay $100$yen to him.
</li>

<li>
Pay $2$yen and press the button at time $3$. This makes the signal green from time $3$to time $4$.
</li>

<li>
Person $3$comes at time $3.5$. Since the signal is green, they pay $100$yen to him.
</li>

</ul>

<p>
In this case, the money received by him minus the cost of pressing the button is $294$yen, and it can be proved that $294$yen is the maximum value.
</p>

<p>
Note that he can press the button at negative times.
</p>

</section>

</div>

</span>

</span>

</div>
