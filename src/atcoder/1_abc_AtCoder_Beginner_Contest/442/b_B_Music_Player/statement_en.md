
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
Takahashi has a music player. Initially, the volume is $0$and the music is stopped.
</p>

<p>
From now on, $Q$operations will be performed in order. The $i$-th operation is represented by an integer $A_i$, which means the following:
</p>

<ul>

<li>
If $A_i = 1$, increase the volume by $1$.
</li>

<li>
If $A_i = 2$, if the current volume is $1$or more, decrease it by $1$; if it is $0$, do nothing.
</li>

<li>
If $A_i = 3$, if the music is stopped, play it; if the music is playing, stop it.
</li>

</ul>

<p>
For $i = 1, 2, \ldots, Q$, solve the following problem:
</p>

<ul>

<li>
Determine whether the music is playing at volume $3$or more immediately after the $i$-th operation.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq Q \leq 2 \times 10^5$
</li>

<li>
$A_i \in \lbrace 1, 2, 3 \rbrace$
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

$Q$$A_1$$A_2$$\vdots$$A_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $i$-th line should contain `Yes`if the music is playing at volume $3$or more immediately after the $i$-th operation, and `No`otherwise.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

10
2
1
3
1
3
1
1
3
2
2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

No
No
No
No
No
No
No
Yes
Yes
No

</div>

<ul>

<li>

<p>
After the $1$-st operation, the volume is $0$and the music is stopped.
</p>

</li>

<li>

<p>
After the $2$-nd operation, the volume is $1$and the music is stopped.
</p>

</li>

<li>

<p>
After the $3$-rd operation, the volume is $1$and the music is playing.
</p>

</li>

<li>

<p>
After the $4$-th operation, the volume is $2$and the music is playing.
</p>

</li>

<li>

<p>
After the $5$-th operation, the volume is $2$and the music is stopped.
</p>

</li>

<li>

<p>
After the $6$-th operation, the volume is $3$and the music is stopped.
</p>

</li>

<li>

<p>
After the $7$-th operation, the volume is $4$and the music is stopped.
</p>

</li>

<li>

<p>
After the $8$-th operation, the volume is $4$and the music is playing.
</p>

</li>

<li>

<p>
After the $9$-th operation, the volume is $3$and the music is playing.
</p>

</li>

<li>

<p>
After the $10$-th operation, the volume is $2$and the music is playing.
</p>

</li>

</ul>

</section>

</div>

</span>

</span>

</div>
