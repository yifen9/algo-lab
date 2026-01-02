
<div>

<span>

<span>

<p>
Score : $550$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$cat towers arranged in a row from left to right, and the height of the $i$-th tower from the left $(1\leq i\leq N)$is $P_i$.

Here, $(P_1,P_2,\ldots,P_N)$is a permutation of $(1,2,\ldots,N)$.

The distance between the $i$-th tower and the $j$-th tower from the left is defined as $\lvert i-j\rvert$.
</p>

<p>
There is one cat, initially on top of the cat tower of height $N$.

Takahashi wants to exercise this cat by repeatedly choosing and removing towers.
</p>

<p>
When Takahashi removes a tower, the cat moves as follows:
</p>

<ul>

<li>
If the cat is not on top of the tower being removed, the cat does not move.
</li>

<li>
If the cat is on top of the tower being removed and at least one of the towers adjacent to the left or right of that tower exists, the cat moves to the tallest tower (excluding the tower being removed) among the towers that can be reached by repeatedly moving to adjacent towers starting from the tower being removed.
At this time, the cat moves the distance between the tower before movement and the tower after movement (the heights of the towers before, after, and during movement do not matter).
</li>

<li>
If the cat is on top of the tower being removed and no towers adjacent to the left or right of that tower exist, the cat jumps into Takahashi's arms, and the exercise ends here. In this case, no movement occurs.
</li>

</ul>

<p>
Here, the spaces between removed towers are not filled in.
That is, the towers adjacent to the $i$-th tower from the left initially are only the $(i-1)$-th and $(i+1)$-th towers from the left (if they exist),
and 
<strong>
they will never become adjacent to other towers due to the removal of other towers
</strong>
afterward.
</p>

<p>
Find the maximum possible total distance the cat moves before the exercise ends.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N\leq 2\times 10^5$
</li>

<li>
$(P_1,P_2,\ldots, P_N)$is a permutation of $(1,2,\ldots,N)$.
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

$N$$P_1$$P_2$$\ldots$$P_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the maximum possible total distance the cat moves before the exercise ends.
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
5 3 4 1 2

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
Initially, the heights of the cat towers are $5,3,4,1,2$from left to right.

Hereafter, the $i$-th cat tower from the left $(1\leq i\leq 5)$is called tower $i$.

Initially, the cat is on tower $1$(height $5$).
</p>

<p>
If Takahashi removes towers in the order $1,2,3,5,4$, the cat moves as follows:
</p>

<ul>

<li>
Takahashi removes tower $1$. The towers that can be reached by only moving to adjacent towers from tower $1$are towers $2,3,4,5$(excluding tower $1$). The cat moves to tower $3$(height $4$), which is the tallest among them.
</li>

<li>
Takahashi removes tower $2$. The cat does not move.
</li>

<li>
Takahashi removes tower $3$. The towers that can be reached by only moving to adjacent towers from tower $3$are towers $4,5$(excluding tower $3$). The cat moves to tower $5$(height $2$), which is the tallest among them.
</li>

<li>
Takahashi removes tower $5$. The towers that can be reached by only moving to adjacent towers from tower $5$are only tower $4$(excluding tower $5$). The cat moves to tower $4$(height $1$).
</li>

<li>
Takahashi removes tower $4$. The cat jumps into Takahashi's arms, and the exercise ends.
</li>

</ul>

<p>
Here, the cat moves the total distance of $\lvert 1-3\rvert+\lvert 3-5\rvert+\lvert 5-4\rvert=5$.
There is no way to remove towers that makes the total distance moved $6$or more, so output $5$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
1 3 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

<p>
Initially, the heights of the cat towers are $1,3,2$from left to right.

Hereafter, the $i$-th cat tower from the left $(1\leq i\leq 3)$is called tower $i$.

Initially, the cat is on tower $2$(height $3$).
</p>

<p>
If Takahashi removes towers in the order $2,3$, the cat moves as follows:
</p>

<ul>

<li>
Takahashi removes tower $2$. The towers that can be reached by only moving to adjacent towers from tower $2$are towers $1,3$(excluding tower $2$). The cat moves to tower $3$(height $2$), which is the tallest among them.
</li>

<li>
Takahashi removes tower $3$. The cat jumps into Takahashi's arms, and the exercise ends.
</li>

</ul>

<p>
Here, the cat moves the total distance of $\lvert 2-3\rvert=1$, which is the maximum.

Note that after removing tower $2$, tower $1$and tower $3$are not considered to be adjacent.
</p>

</section>

</div>

</span>

</span>

</div>
