
<div>

<span>

<span>

<p>
Score: $100$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Team Takahashi and Team Aoki are playing a baseball game, with Team Takahashi batting first.

Currently, the game has finished through the top of the ninth inning, and the bottom of the ninth is about to begin.
</p>

<p>
Team Takahashi scored $A_i$runs in the top of the $i$-th inning $(1\leq i\leq 9)$, and Team Aoki scored $B_j$runs in the bottom of the $j$-th inning $(1\leq j\leq 8)$.

At the end of the top of the ninth, Team Takahashi's score is not less than Team Aoki's score.

Determine the minimum number of runs Team Aoki needs to score in the bottom of the ninth to win the game.
</p>

<p>
Here, if the game is tied at the end of the bottom of the ninth, it results in a draw. Therefore, for Team Aoki to win, they must score strictly more runs than Team Takahashi by the end of the bottom of the ninth.

Team Takahashi's score at any point is the total runs scored in the tops of the innings up to that point, and Team Aoki's score is the total runs scored in the bottoms of the innings.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$0\leq A_i, B_j\leq 99$
</li>

<li>
$A_1 + A_2 + A_3 + A_4 + A_5 + A_6 + A_7 + A_8 + A_9 \geq B_1 + B_2 + B_3 + B_4 + B_5 + B_6 + B_7 + B_8$
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

$A_1$$A_2$$A_3$$A_4$$A_5$$A_6$$A_7$$A_8$$A_9$$B_1$$B_2$$B_3$$B_4$$B_5$$B_6$$B_7$$B_8$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the minimum number of runs Team Aoki needs to score in the bottom of the ninth inning to win.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

0 1 0 1 2 2 0 0 1
1 1 0 0 0 0 1 0

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
At the end of the top of the ninth inning, Team Takahashi has scored seven runs, and Team Aoki has scored three runs.

Therefore, if Team Aoki scores five runs in the bottom of the ninth, the scores will be $7-8$, allowing them to win.

Note that scoring four runs would result in a draw and not a victory.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

</section>

</div>

</span>

</span>

</div>
