
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
AtCoder Inc. starts work at time $0$and ends work at time $T$. The interval between time $t$and time $t+1$is $1$second.

Takahashi-kun views the SNS chokutter during AtCoder Inc.'s business hours according to the following rules:
</p>

<ul>

<li>
He opens chokutter at the same time as work starts.
</li>

<li>
If chokutter is open at the moment Aoki-kun passes behind Takahashi-kun's desk, he immediately closes it.
</li>

<li>
If Takahashi-kun closes chokutter at time $t$, he always opens it at time $t+100$.
</li>

</ul>

<p>
From the start to the end of work, Aoki-kun passed behind Takahashi-kun's desk $N$times, with the $i$-th time being at time $A_i$.

From the start to the end of work, for how many seconds in total was Takahashi-kun viewing chokutter?


<strong>
Aoki-kun never passed behind the desk at the moment when Takahashi-kun opened chokutter.
</strong>

</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
All input values are integers.
</li>

<li>
$0 \le N \le 3 \times 10^5$
</li>

<li>
$1 \le A_1 < A_2 < \dots < A_N \le T \le 10^9$
</li>

<li>
Aoki-kun never passes behind the desk at the moment when Takahashi-kun opens chokutter.
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

$N$$T$$A_1$$A_2$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 700
100 150 300 350 700

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

500

</div>

<ul>

<li>
At time $0$, Takahashi-kun opens chokutter.
</li>

<li>
At time $100$, Aoki-kun passes behind Takahashi-kun's desk, and Takahashi-kun immediately closes chokutter.
</li>

<li>
At time $150$, Aoki-kun passes behind Takahashi-kun's desk, but Takahashi-kun does not have chokutter open at this time.
</li>

<li>
At time $200$, Takahashi-kun opens chokutter again.
</li>

<li>
At time $300$, Aoki-kun passes behind Takahashi-kun's desk, and Takahashi-kun immediately closes chokutter.
</li>

<li>
At time $350$, Aoki-kun passes behind Takahashi-kun's desk, but Takahashi-kun does not have chokutter open at this time.
</li>

<li>
At time $400$, Takahashi-kun opens chokutter again.
</li>

<li>
At time $700$, Aoki-kun passes behind Takahashi-kun's desk, and Takahashi-kun immediately closes chokutter.
</li>

</ul>

<p>
Takahashi-kun was viewing chokutter for a total of $500$seconds.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

0 1000000000


</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1000000000

</div>

<p>
There may be cases where Aoki-kun never passes behind Takahashi-kun's desk.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10 1234
395 424 588 745 773 863 910 958 1102 1195

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

734

</div>

</section>

</div>

</span>

</span>

</div>
