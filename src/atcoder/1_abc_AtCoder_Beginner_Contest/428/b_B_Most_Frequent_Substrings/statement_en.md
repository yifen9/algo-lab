
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
You are given a string $S$of length $N$consisting of lowercase English letters.
</p>

<p>
Define the 
<strong>
number of occurrences
</strong>
of a string $t$of length $K$as the number of integers $i$that satisfy the following condition:
</p>

<ul>

<li>
$1 \leq i \leq N-K+1$
</li>

<li>
The substring of $S$from the $i$-th character to the $(i+K-1)$-th character matches $t$.
</li>

</ul>

<p>
Find the maximum value $x$of the number of occurrences of a string of length $K$.
Also, output all strings of length $K$with $x$occurrences in ascending lexicographical order.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$N, K$are integers.
</li>

<li>
$S$is a string of length $N$consisting of lowercase English letters.
</li>

<li>
$1 \leq K \leq N \leq 100$
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

$N$$K$$S$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output two lines.
</p>

<p>
The first line should contain the maximum value $x$of the number of occurrences of a string of length $K$.
</p>

<p>
The second line should contain all strings of length $K$with $x$occurrences in ascending lexicographical order, separated by spaces.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

9 3
ovowowovo

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
ovo owo

</div>

<p>
The following strings have two occurrences:
</p>

<ul>

<li>
For the string `ovo`, $i=1,7$satisfy the condition, so the number of occurrences of `ovo`is $2$.
</li>

<li>
For the string `owo`, $i=3,5$satisfy the condition, so the number of occurrences of `owo`is $2$.
</li>

</ul>

<p>
There is no string of length $3$with more than two occurrences, so the maximum value is $2$.
</p>

<p>
On the other hand, the following are examples of strings with fewer than two occurrences:
</p>

<ul>

<li>
For the string `vow`, $i=2$satisfies the condition, so the number of occurrences of `vow`is $1$.
</li>

<li>
For the string `ooo`, there is no $i$that satisfies the condition, so the number of occurrences of `ooo`is $0$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

9 1
ovowowovo

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

5
o

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

35 3
thequickbrownfoxjumpsoverthelazydog

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

2
the

</div>

</section>

</div>

</span>

</span>

</div>
