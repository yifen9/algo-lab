
<div>

<span>

<span>

<p>
Score : $150$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Takahashi is enjoying a game at school. The game starts at the moment the bell rings.
</p>

<p>
Immediately after the bell rings, he repeats the following actions:
</p>

<ul>

<li>
Run at a speed of $S$meters per second for $A$seconds. Then, remain stationary for $B$seconds.
</li>

</ul>

<p>
How many meters in total does he run by the time $X$seconds have elapsed since the bell rang?
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq S \leq 15$
</li>

<li>
$1 \leq A \leq 1000$
</li>

<li>
$1 \leq B \leq 1000$
</li>

<li>
$1 \leq X \leq 1000$
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

$S$$A$$B$$X$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer in one line. Omit the unit (meters) in the output.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

7 3 2 11

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

49

</div>

<p>
During the $11$seconds after the bell rings, Takahashi moves as follows:
</p>

<ul>

<li>
From $0$seconds to $3$seconds, he runs at a speed of $7$meters per second. The distance traveled during this time is $21$meters.
</li>

<li>
From $3$seconds to $5$seconds, he remains stationary.
</li>

<li>
From $5$seconds to $8$seconds, he runs at a speed of $7$meters per second. The distance traveled during this time is $21$meters.
</li>

<li>
From $8$seconds to $10$seconds, he remains stationary.
</li>

<li>
From $10$seconds to $11$seconds, he runs at a speed of $7$meters per second. The distance traveled during this time is $7$meters.
</li>

</ul>

<p>
The total distance traveled is $49$meters, so output $49$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6 3 2 9

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

36

</div>

<p>
During the $9$seconds after the bell rings, Takahashi moves as follows:
</p>

<ul>

<li>
From $0$seconds to $3$seconds, he runs at a speed of $6$meters per second. The distance traveled during this time is $18$meters.
</li>

<li>
From $3$seconds to $5$seconds, he remains stationary.
</li>

<li>
From $5$seconds to $8$seconds, he runs at a speed of $6$meters per second. The distance traveled during this time is $18$meters.
</li>

<li>
From $8$seconds to $9$seconds, he remains stationary.
</li>

</ul>

<p>
The total distance traveled is $36$meters, so output $36$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

1 1 666 428

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

1

</div>

<p>
During the $428$seconds after the bell rings, Takahashi moves as follows:
</p>

<ul>

<li>
From $0$seconds to $1$second, he runs at a speed of $1$meter per second. The distance traveled during this time is $1$meter.
</li>

<li>
From $1$second to $428$seconds, he remains stationary.
</li>

</ul>

<p>
The total distance traveled is $1$meter, so output $1$.
</p>

</section>

</div>

</span>

</span>

</div>
