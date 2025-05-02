
<div>

<span>

<span>

<p>
Score : $700$points
</p>

<div>

<section>

### **Problem Statement**

<p>
We have a sandglass consisting of two bulbs, bulb A and bulb B. These bulbs contain some amount of sand.
When we put the sandglass, either bulb $A$or $B$lies on top of the other and becomes the 
<em>
upper bulb
</em>
. The other bulb becomes the 
<em>
lower bulb
</em>
.
</p>

<p>
The sand drops from the upper bulb to the lower bulb at a rate of $1$gram per second.
When the upper bulb no longer contains any sand, nothing happens.
</p>

<p>
Initially at time $0$, bulb A is the upper bulb and contains $a$grams of sand; bulb B contains $X-a$grams of sand (for a total of $X$grams).
</p>

<p>
We will turn over the sandglass at time $r_1,r_2,..,r_K$. Assume that this is an instantaneous action and takes no time. Here, time $t$refer to the time $t$seconds after time $0$.
</p>

<p>
You are given $Q$queries.
Each query is in the form of $(t_i,a_i)$.
For each query, assume that $a=a_i$and find the amount of sand that would be contained in bulb A at time $t_i$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1≤X≤10^9$
</li>

<li>
$1≤K≤10^5$
</li>

<li>
$1≤r_1<r_2< .. <r_K≤10^9$
</li>

<li>
$1≤Q≤10^5$
</li>

<li>
$0≤t_1<t_2< .. <t_Q≤10^9$
</li>

<li>
$0≤a_i≤X (1≤i≤Q)$
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

$X$$K$$r_1$$r_2$.. $r_K$$Q$$t_1$$a_1$$t_2$$a_2$$:$$t_Q$$a_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
For each query, print the answer in its own line.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

180
3
60 120 180
3
30 90
61 1
180 180

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

60
1
120

</div>

<p>
In the first query, $30$out of the initial $90$grams of sand will drop from bulb A, resulting in $60$grams.
In the second query, the initial $1$gram of sand will drop from bulb A, and nothing will happen for the next $59$seconds. Then, we will turn over the sandglass, and $1$second after this, bulb $A$contains $1$gram of sand at the time in question.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

100
1
100000
4
0 100
90 100
100 100
101 100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

100
10
0
0

</div>

<p>
In every query, the upper bulb initially contains $100$grams, and the question in time comes before we turn over the sandglass.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

100
5
48 141 231 314 425
7
0 19
50 98
143 30
231 55
342 0
365 100
600 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

19
52
91
10
58
42
100

</div>

</section>

</div>

</span>

</span>

</div>
