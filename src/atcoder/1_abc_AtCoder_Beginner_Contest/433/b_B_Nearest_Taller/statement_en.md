
<div>

<span>

<span>

<p>
Score : $200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$people standing in a row from left to right. The $i$-th person from the left $(1\le i\le N)$is called person $i$. The height of person $i$$(1\le i\le N)$is $A_i$.
</p>

<p>
For each $i=1,2,\ldots,N$, determine whether there exists a person to the left of person $i$who is taller than person $i$, and if so, find the person standing closest to person $i$among them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le 100$
</li>

<li>
$1\le A_i\le 100$
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
Output $N$lines.
</p>

<p>
The $i$-th line $(1\le i\le N)$should contain $-1$if there is no person to the left of person $i$who is taller than person $i$, and otherwise, the number representing the person standing closest to person $i$among such people.
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
4 3 2 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

-1
1
2
-1

</div>

<ul>

<li>
There is no person to the left of person $1$. Thus, output $-1$on the first line.
</li>

<li>
Among the people to the left of person $2$, only person $1$is taller than person $2$. Thus, output $1$on the second line.
</li>

<li>
Among the people to the left of person $3$, persons $1,2$are taller than person $3$, and the person standing closest to person $3$is person $2$. Thus, output $2$on the third line.
</li>

<li>
There is no person to the left of person $4$who is taller than person $4$. Thus, output $-1$on the fourth line.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
7 7 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1
-1
-1

</div>

<p>
There may be multiple people with the same height.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

6
31 9 17 10 2 9

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

-1
1
1
3
4
4

</div>

</section>

</div>

</span>

</span>

</div>
