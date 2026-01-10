
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
Halloween season has arrived. As a test of courage, you are about to challenge a haunted house.
</p>

<p>
There is a haunted house with $F$floors, and each floor is represented by an $H$-row by $W$-column grid. Let cell $(k,i,j)$be the cell at the $i$-th row from the top and $j$-th column from the left of the grid representing floor $k$.
</p>

<p>
The content of cell $(k,i,j)$is represented by the character $S_{k,i,j}$as follows:
</p>

<ul>

<li>
If $S_{k,i,j}$is a digit (`0`- `9`), cell $(k,i,j)$is an empty cell with a number of coins equal to the single-digit integer represented by the digit.
</li>

<li>
If $S_{k,i,j}$is `#`, cell $(k,i,j)$is a wall cell.
</li>

</ul>

<p>
You can move directly from an empty cell $(k,i,j)$to another cell $(k', i', j')$if cell $(k', i', j')$is an empty cell and one of the following is satisfied:
</p>

<ul>

<li>
$k' = k$and $|i' - i| + |j' - j| = 1$are satisfied.
</li>

<li>
$(k', i', j') = (k+1, i, j)$is satisfied.
</li>

<li>
$(k', i', j') = (k-1, i, j)$is satisfied, and a 
<strong>
ladder
</strong>
is placed at cell $(k,i,j)$.
</li>

</ul>

<p>
You cannot move outside the grid.
</p>

<p>
You are given $Q$questions; answer each of them. The $i$-th question ($1 \leq i \leq Q$) is as follows:
</p>

<ul>

<li>
Find the maximum total number of coins in the cells you visit if you choose exactly one empty cell and place a ladder there, start at cell $(G_i, A_i, B_i)$, and repeatedly move.
</li>

</ul>

<p>
Each question is independent. That is, a ladder placed for one question does not affect other questions.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$F,H,W$are integers.
</li>

<li>
$1 \leq F \leq 10$
</li>

<li>
$1 \leq H,W \leq 500$
</li>

<li>
$S_{k,i,j}$is either a digit (`0`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`) or `#`. ($1 \leq k \leq F, 1 \leq i \leq H, 1 \leq j \leq W$)
</li>

<li>
$Q$is an integer.
</li>

<li>
$1 \leq Q \leq 10^5$
</li>

<li>
$G_i, A_i, B_i$are integers. ($1 \leq i \leq Q$)
</li>

<li>
$1 \leq G_i \leq F$($1 \leq i \leq Q$)
</li>

<li>
$1 \leq A_i \leq H$($1 \leq i \leq Q$)
</li>

<li>
$1 \leq B_i \leq W$($1 \leq i \leq Q$)
</li>

<li>
$S_{G_i, A_i, B_i}$is not `#`. ($1 \leq i \leq Q$)
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

$F$$H$$W$$S_{1,1,1} S_{1,1,2} \cdots S_{1,1,W}$$S_{1,2,1} S_{1,2,2} \cdots S_{1,2,W}$$\vdots$$S_{1,H,1} S_{1,H,2} \cdots S_{1,H,W}$$S_{2,1,1} S_{2,1,2} \cdots S_{2,1,W}$$S_{2,2,1} S_{2,2,2} \cdots S_{2,2,W}$$\vdots$$S_{2,H,1} S_{2,H,2} \cdots S_{2,H,W}$$\vdots$$S_{F,1,1} S_{F,1,2} \cdots S_{F,1,W}$$S_{F,2,1} S_{F,2,2} \cdots S_{F,2,W}$$\vdots$$S_{F,H,1} S_{F,H,2} \cdots S_{F,H,W}$$Q$$G_1$$A_1$$B_1$$G_2$$A_2$$B_2$$\vdots$$G_Q$$A_Q$$B_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $i$-th line ($1 \leq i \leq Q$) should contain the answer to the $i$-th question.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 5 6
######
##5###
#1#11#
#1#11#
######
######
##313#
#4##1#
#242##
######
######
#0####
##4###
###99#
######
3
1 2 3
2 3 2
3 2 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

47
34
0

</div>

<p>
For the first question, by placing a ladder at cell $(2,3,5)$and moving as follows, you can make the total number of coins in the visited cells $47$:
</p>

<ol>

<li>
Start at cell $(1,2,3)$on the first floor.
</li>

<li>
Go up to the second floor and move in the order $(2,2,3) \to (2,2,4) \to (2,2,5) \to (2,3,5)$.
</li>

<li>
Go down to the first floor and move in the order $(1,3,5) \to (1,4,5) \to (1,4,4) \to (1,3,4) \to (1,4,4)$.
</li>

<li>
Go up to the second floor and move in the order $(2,4,4) \to (2,4,3) \to (2,4,2) \to (2,3,2) \to (2,4,2) \to (2,4,3) \to (2,4,4)$.
</li>

<li>
Go up to the third floor and move in the order $(3,4,4) \to (3,4,5)$.
</li>

</ol>

<p>
For the second question, by placing a ladder at cell $(2,4,4)$and moving as follows, you can make the total number of coins in the visited cells $34$:
</p>

<ol>

<li>
Move in the order $(2,3,2) \to (2,4,2) \to (2,4,3) \to (2,4,4)$on the second floor.
</li>

<li>
Go down to the first floor and move in the order $(1,4,4) \to (1,4,5) \to (1,3,5) \to (1,3,4) \to (1,4,4)$.
</li>

<li>
Go up to the second floor and be at cell $(2,4,4)$.
</li>

<li>
Go up to the third floor and move in the order $(3,4,4) \to (3,4,5)$.
</li>

</ol>

<p>
For the third question, no matter how you place the ladder, you cannot move from the starting cell $(3,2,2)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 6 30
31#990#7###71298#6#9####3##04#
###66###6######7#4#3#1079239#6
891###8#73#7#5838#589#225#1282
#####5#306#9#38#50##6#71##8658
6#68#4#5###30###3#5716987#####
06#8####3#####134#5##2##28#169
#5#11####0#75#8######28#6#904#
85#71####0##9#7#0##8#2##00####
#1#09#3772#838#67#6##261###0#4
#4##78###7#########9#9#488##08
43#1##4632##46714436##849#77#6
8#83#61##4#14476#9#1##72#3####
5#99####52##6#9####9#4#4132#3#
##910#27529#69##491###0#06#9##
0#60845#02##28##610#2####25#6#
#229156374##47#30907#60#####28
#0#810#54###21##1#3###8#5917##
###6#56#60##04#73###6255###2##
10
3 4 23
3 2 4
1 4 14
2 3 12
1 1 16
1 2 9
3 5 6
1 3 19
2 2 4
3 4 9

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

136
217
474
255
474
285
217
451
251
217

</div>

</section>

</div>

</span>

</span>

</div>
