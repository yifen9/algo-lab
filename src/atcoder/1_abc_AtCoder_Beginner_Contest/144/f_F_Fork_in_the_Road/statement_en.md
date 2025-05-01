
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
There is a cave consisting of $N$rooms and $M$one-directional passages. The rooms are numbered $1$through $N$.
</p>

<p>
Takahashi is now in Room $1$, and Room $N$has the exit. The $i$-th passage connects Room $s_i$and Room $t_i$($s_i$< $t_i$) and can only be traversed in the direction from Room $s_i$to Room $t_i$. It is known that, for each room except Room $N$, there is at least one passage going from that room.
</p>

<p>
Takahashi will escape from the cave. Each time he reaches a room (assume that he has reached Room $1$at the beginning), he will choose a passage uniformly at random from the ones going from that room and take that passage.
</p>

<p>
Aoki, a friend of Takahashi's, can block one of the passages (or do nothing) before Takahashi leaves Room $1$. However, it is not allowed to block a passage so that Takahashi is potentially unable to reach Room $N$.
</p>

<p>
Let $E$be the expected number of passages Takahashi takes before he reaches Room $N$. Find the value of $E$when Aoki makes a choice that minimizes $E$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 600$
</li>

<li>
$N-1 \leq M \leq \frac{N(N-1)}{2}$
</li>

<li>
$s_i < t_i$
</li>

<li>
If $i != j$, $(s_i, t_i) \neq (s_j, t_j)$. 
<strong>
(Added 21:23 JST)
</strong>

</li>

<li>
For every $v = 1, 2, ..., N-1$, there exists $i$such that $v = s_i$.
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
Input is given from Standard Input in the following format:
</p>

<div>

$N$$M$$s_1$$t_1$$:$$s_M$$t_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the value of $E$when Aoki makes a choice that minimizes $E$.
Your output will be judged as correct when the absolute or relative error from the judge's output is at most $10^{-6}$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 6
1 4
2 3
1 3
1 2
3 4
2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1.5000000000

</div>

<p>
If Aoki blocks the passage from Room $1$to Room $2$, Takahashi will go along the path `1`→ `3`→ `4`with probability $\frac{1}{2}$and `1`→ `4`with probability $\frac{1}{2}$. $E = 1.5$here, and this is the minimum possible value of $E$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 2
1 2
2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

2.0000000000

</div>

<p>
Blocking any one passage makes Takahashi unable to reach Room $N$, so Aoki cannot block a passage.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10 33
3 7
5 10
8 9
1 10
4 6
2 5
1 7
6 10
1 4
1 3
8 10
1 5
2 6
6 9
5 6
5 8
3 6
4 8
2 7
2 9
6 7
1 2
5 9
6 8
9 10
3 9
7 8
4 5
2 10
5 7
3 5
4 7
4 9

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

3.0133333333

</div>

</section>

</div>

</span>

</span>

</div>
