
<div>

<span>

<span>

<p>
Score : $800$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Takahashi and Aoki will play a game using a grid with $H$rows and $W$columns of square cells.
There are $N$obstacles on this grid; the $i$-th obstacle is at $(X_i,Y_i)$.
Here, we represent the cell at the $i$-th row and $j$-th column $(1 \leq i \leq H, 1 \leq j \leq W)$by $(i,j)$.
There is no obstacle at $(1,1)$, and there is a piece placed there at $(1,1)$.
</p>

<p>
Starting from Takahashi, he and Aoki alternately perform one of the following actions:
</p>

<ul>

<li>
Move the piece to an adjacent cell.
    Here, let the position of the piece be $(x,y)$. Then Takahashi can only move the piece to $(x+1,y)$, and Aoki can only move the piece to $(x,y+1)$.
    If the destination cell does not exist or it is occupied by an obstacle, this action cannot be taken.
</li>

<li>
Do not move the piece, and end his turn without affecting the grid.
</li>

</ul>

<p>
The game ends when the piece does not move twice in a row.
</p>

<p>
Takahashi would like to perform as many actions (including not moving the piece) as possible before the game ends, while Aoki would like to perform as few actions as possible before the game ends.
How many actions will Takahashi end up performing?
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq H,W \leq 2\times 10^5$
</li>

<li>
$0 \leq N \leq 2\times 10^5$
</li>

<li>
$1 \leq X_i \leq H$
</li>

<li>
$1 \leq Y_i \leq W$
</li>

<li>
If $i \neq j$, $(X_i,Y_i) \neq (X_j,Y_j)$
</li>

<li>
$(X_i,Y_i) \neq (1,1)$
</li>

<li>
$X_i$and $Y_i$are integers.
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

$H$$W$$N$$X_1$$Y_1$$:$$X_N$$Y_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the number of actions Takahashi will end up performing.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 3 1
3 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2

</div>

<p>
For example, the game proceeds as follows:
</p>

<ul>

<li>
Takahashi moves the piece to (2,1).
</li>

<li>
Aoki does not move the piece.
</li>

<li>
Takahashi moves the piece to (3,1).
</li>

<li>
Aoki does not move the piece.
</li>

<li>
Takahashi does not move the piece.
</li>

</ul>

<p>
Takahashi performs three actions in this case, but if both players play optimally, Takahashi will perform only two actions before the game ends.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 10 14
4 3
2 2
7 3
9 10
7 7
8 1
10 10
5 4
3 4
2 8
6 4
4 4
5 8
9 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

6

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

100000 100000 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

100000

</div>

</section>

</div>

</span>

</span>

</div>
