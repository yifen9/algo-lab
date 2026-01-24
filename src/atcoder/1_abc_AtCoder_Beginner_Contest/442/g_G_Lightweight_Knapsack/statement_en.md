
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$types of items.
The $i$-th type of item has 
<strong>
weight
</strong>
$W_i$and 
<strong>
value
</strong>
$V_i$, and you have $K_i$of them.
</p>

<p>
When choosing some (possibly zero) items from these $K_1+\dots+K_N$items so that the total weight does not exceed $C$, find the maximum possible total value of the chosen items.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N \leq 2\times 10^5$
</li>

<li>
$1\leq C \leq 2\times 10^9$
</li>

<li>

<span>
$1\leq W_i \leq 3$
</span>

</li>

<li>
$1\leq V_i \leq 10^9$
</li>

<li>
$1\leq K_i \leq 10^9$
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

$N$$C$$W_1$$V_1$$K_1$$W_2$$V_2$$K_2$$\vdots$$W_N$$V_N$$K_N$
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

4 7
3 5 5
1 2 4
2 7 1
2 1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

16

</div>

<p>
If you choose $1$item of the $1$-st type, $2$items of the $2$-nd type, and $1$item of the $3$-rd type, the total weight is $3\times 1+1\times 2+2\times 1=7\ (\leq C)$and
the total value is $5\times 1+2\times 2+7\times 1=16$, which is the maximum.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2 1
3 442 442
2 442 442

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

<p>
You cannot choose any items.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

15 913575467
1 60505998 818008580
2 121011861 138996221
3 181517958 501899080
1 60506027 840594328
3 181517875 350034067
1 60505924 155374934
3 181517816 910748511
1 60506042 545531545
3 181517877 797829355
3 181517837 164163676
1 60505894 353195922
1 60505912 954291757
1 60506022 160449218
3 181517873 404011431
1 60506043 782177068

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

55276836358648682

</div>

</section>

</div>

</span>

</span>

</div>
