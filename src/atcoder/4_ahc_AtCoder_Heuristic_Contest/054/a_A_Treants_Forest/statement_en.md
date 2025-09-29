
<div>

<span>

<span>

<div>

<section>

### **Story**

<p>
To the south of the Kingdom of AtCoder lies a mysterious forest commonly known as the "Lost Forest," where the paths change every time one enters.
It is said that within this forest blooms a legendary flower called 
<em>
Aura Amaryllis
</em>
(commonly abbreviated as AA), which brings happiness to those who find it. Even today, adventurers arrive in search of this flower.
</p>

<p>
The true nature of the Lost Forest is that tree monsters known as "Treants" disguise themselves as trees to confuse adventurers. Treants sustain their lives by absorbing magical energy from lost adventurers, so they aim to keep the adventurers in the forest for as long as possible.
However, if an adventurer fails to reach the AA, rumors will spread that "the flower never existed," and no one will enter the forest again. If that happens, the Treants will no longer be able to obtain magical energy and will eventually perish.
</p>

<p>
Furthermore, adventurers explore the forest while mapping it to avoid getting lost. If a Treant moves to a location that has already been mapped, the adventurer will realize that it is not a real tree but a Treant in disguise and will cut it down. This situation must be avoided at all costs.
</p>

<p>
As the boss of the Treants, your role is to adjust the placement of the Treants in response to the adventurer's movements to ensure that it takes longer for the adventurer to reach the AA.
</p>

</section>

</div>

<div>

<section>

### **Problem Statement**

<p>
There is a forest consisting of an $N \times N$grid of cells.
The coordinates of the top-left cell are $(0, 0)$. The cell located $i$cells down and $j$cells to the right has coordinates $(i, j)$.
Each cell is either an "empty cell" or a "tree". The area outside the $N \times N$grid is surrounded by trees.
</p>

<p>
The cell $(0, \lfloor \frac{N}{2} \rfloor)$is the entrance to the forest and is an empty cell.
The legendary flower blooms at cell $(t_i, t_j)$, which is also an empty cell.
</p>

<p>
An adventurer has entered the forest in search of the legendary flower.
The adventurer has three states: the 
<strong>
current position
</strong>
and the 
<strong>
revealed cells
</strong>
, which are public information, and the 
<strong>
destination
</strong>
, which is hidden.
A map of the forest assuming all unrevealed cells are empty is called the 
<strong>
tentative map
</strong>
.
</p>

<p>
Initially, the 
<strong>
current position
</strong>
is the forest entrance, the 
<strong>
revealed cells
</strong>
include only that one cell and all cells outside the $N \times N$grid, and the 
<strong>
destination
</strong>
is unset.
Each turn, the adventurer's actions are processed in the following order:
</p>

<ol>

<li>
If the legendary flower is at the 
<strong>
current position
</strong>
, the goal is achieved and the adventurer stops moving.
</li>

<li>
For each of the four directions (up, down, left, right), add to the 
<strong>
revealed cells
</strong>
all unrevealed cells from the 
<strong>
current position
</strong>
up to and including the first "tree" cell encountered in that direction.
</li>

<li>
If the legendary flower is included in the 
<strong>
revealed cells
</strong>
, set the 
<strong>
destination
</strong>
to that cell.
</li>

<li>
If the 
<strong>
destination
</strong>
is set but is unreachable from the current position in the 
<strong>
tentative map
</strong>
using only empty cells, unset the 
<strong>
destination
</strong>
.
</li>

<li>
If the 
<strong>
destination
</strong>
is unset or is a cell in the 
<strong>
revealed cells
</strong>
other than the legendary flower, choose one cell uniformly at random from the unrevealed cells that are reachable from the current position via empty cells in the 
<strong>
tentative map
</strong>
, and set it as the 
<strong>
destination
</strong>
(if no such cell exists, this will result in a 
<span>
WA
</span>
, as described below).
</li>

<li>
In the 
<strong>
tentative map
</strong>
, compute the shortest distance to the 
<strong>
destination
</strong>
using only empty cells. Move to an adjacent empty cell that shortens the distance to the 
<strong>
destination
</strong>
. If multiple such cells exist, choose the one in the order of preference: up, down, left, right.
</li>

</ol>

<p>
As the boss of the tree monsters known as "Treants," your goal is to direct the Treants to confuse the adventurer and maximize the number of turns it takes to reach the legendary flower.
</p>

<p>
At the beginning of each turn, you may choose any number of empty cells that are not part of the 
<strong>
revealed cells
</strong>
and place one Treant in each.
Cells where Treants are placed are no longer considered "empty" and are treated as "trees" from that point onward. Treants cannot be moved once placed.
</p>

<p>
You must ensure that there is always at least one path from the forest entrance to the legendary flower consisting only of empty cells.
If no such path exists, your solution will result in a 
<span>
WA
</span>
.
</p>

</section>

</div>

<div>

<section>

### **Scoring**

<p>
The number of moves the adventurer takes to reach the legendary flower from the forest entrance is the absolute score for that test case.

The higher the absolute score, the better.
</p>

<p>
For each test case, we compute the 
<font color="red">
<strong>
relative score
</strong>
</font>
$\mathrm{round}(10^9\times \frac{\mathrm{YOUR}}{\mathrm{MAX}})$, where YOUR is your absolute score and MAX is the highest absolute score among all competitors obtained on that test case. The score of the submission is the sum of the relative scores.
</p>

<p>
The final ranking will be determined by the system test with more inputs which will be run after the contest is over.
In both the provisional/system test, if your submission produces illegal output or exceeds the time limit for some test cases, only the score for those test cases will be zero, and your submission will be excluded from the MAX calculation for those test cases.
</p>

<p>
The system test will be performed only for 
<font color="red">
<strong>
the last submission which received a result other than 
<span>
CE
</span>

</strong>
</font>
.
Be careful not to make a mistake in the final submission.
</p>

#### **Number of test cases**

<ul>

<li>
Provisional test: 100
</li>

<li>
System test: 3000. We will publish <a href="https://img.atcoder.jp/ahc054/seeds.txt">seeds.txt</a>(sha256=f46e04db0ec8f80d641bbc8e166b1d2f4050a340b356acea1adce1a41a0a7fc8) after the contest is over.
</li>

</ul>

#### **About relative evaluation system**

<p>
In both the provisional/system test, the standings will be calculated using only the last submission which received a result other than 
<span>
CE
</span>
.
Only the last submissions are used to calculate the MAX for each test case when calculating the relative scores.
</p>

<p>
The scores shown in the standings are relative, and whenever a new submission arrives, all relative scores are recalculated.
On the other hand, the score for each submission shown on the submissions page is the sum of the absolute score for each test case, and the relative scores are not shown.
In order to know the relative score of submission other than the latest one in the current standings, you need to resubmit it.
If your submission produces illegal output or exceeds the time limit for some test cases, the score shown on the submissions page will be 0, but the standings show the sum of the relative scores for the test cases that were answered correctly.
</p>

#### **About execution time**

<p>
Execution time may vary slightly from run to run.
In addition, since system tests simultaneously perform a large number of executions, it has been observed that execution time increases by several percent compared to provisional tests.
For these reasons, submissions that are very close to the time limit may result in 
<span>
TLE
</span>
in the system test.
Please measure the execution time in your program to terminate the process, or have enough margin in the execution time.
</p>

</section>

</div>

<div>

<section>

### **Input and Output**

<p>
At the beginning, the following information is given via Standard Input:
</p>

<div>

$N$$t_i$$t_j$$b_{0,0}\cdots b_{0,N-1}$$\vdots$$b_{N-1,0}\cdots b_{N-1,N-1}$
</div>

<ul>

<li>
$N$is the width and height of the forest and satisfies $20 \leq N \leq 40$.
</li>

<li>
$(t_i, t_j)$is the coordinate of the legendary flower and satisfies $0 \leq t_i, t_j \leq N - 1$, with a guaranteed Manhattan distance of at least 5 from the forest entrance $(0, \lfloor \frac{N}{2} \rfloor)$.
</li>

<li>
$b_{i,0} \cdots b_{i,N-1}$is a string of length $N$, where the $j$-th character $b_{i,j}$is `.`if cell $(i, j)$is an empty cell, and `T`if it is a tree.
</li>

<li>
It is guaranteed that every empty cell is reachable from the forest entrance $(0, \lfloor \frac{N}{2} \rfloor)$by traversing only through empty cells.
</li>

</ul>

<p>
Next, repeat the following process.

At the beginning of each turn, the adventurer's current position and the cells newly revealed in the previous turn are given via Standard Input in the following format:
</p>

<div>

$p_i$$p_j$$n$$x_0$$y_0$$\cdots$$x_{n-1}$$y_{n-1}$
</div>

<ul>

<li>
$(p_i, p_j)$is the adventurer's current position.
</li>

<li>
$n$is the number of cells that were newly revealed in the previous turn, and $(x_k, y_k)$represents the coordinates of the $k$-th such cell.
</li>

<li>
On the first turn, $(p_i, p_j) = (0, \lfloor \frac{N}{2} \rfloor)$, $n = 1$, and $(x_0, y_0) = (0, \lfloor \frac{N}{2} \rfloor)$.
</li>

</ul>

<p>
If $(p_i, p_j) = (t_i, t_j)$, it means the adventurer has reached the legendary flower. In that case, terminate the loop and end the program.

Otherwise, let $(x_0', y_0'), \cdots, (x_{m-1}', y_{m-1}')$be the set of cells where Treants will be placed before the start of this turn, and output the following format to Standard Output:
</p>

<div>

$m$$x_0'$$y_0'$$\cdots$$x_{m-1}'$$y_{m-1}'$
</div>

<p>

<font color="red">
<strong>
The output must be followed by a new line, and you have to flush Standard Output.
</strong>
</font>
Otherwise, the submission might be judged as 
<span>
TLE
</span>
.
</p>

<p>

<font color="red">
<strong>
(2025/9/21 06:00 UTC Update)
</strong>
</font>
The execution time limit includes not only the contestant's solution program but also the judge-side tester program.
In this problem setting, it is difficult for the solution program to terminate at an arbitrary timing, so the following cutoff output specification has been added to make it easier to avoid 
<span>
TLE
</span>
.
</p>

<p>

<strong>
Cutoff Output
</strong>
: Instead of outputting the set of cells where new Treants are placed in the above format, the program may output a line containing only `-1`and then terminate immediately.
In that case, the subsequent turns will be treated as if the output had been $m=0$until the adventurer finds the legendary flower, and the execution time spent by the tester on that processing will not be counted toward the time limit.
</p>

<p>
<a href="https://img.atcoder.jp/ahc054/YDAxDRZr_v2.html?lang=en&seed=0&output=sample">Show example</a>
</p>

</section>

</div>

<div>

<section>

### **Input Generation**

<p>
Let $\mathrm{rand}(L, U)$be a function that generates a uniformly random integer between $L$and $U$, inclusive.
</p>

<p>
Generate the forest size $N$by $N = \mathrm{rand}(20, 40)$.
</p>

<p>
Start with all cells as empty, and generate the tree placement using the following procedure:

First, determine the maximum number of trees $K$by $K = \max(1, \mathrm{rand}(0, \lfloor N^2 / 6 \rfloor))$.

List the $N^2 - 1$cells excluding the forest entrance in a random order as $(i_0, j_0), \cdots, (i_{N^2 - 2}, j_{N^2 - 2})$, and for each $k$, perform the following:
</p>

<p>
Tentatively place a tree at $(i_k, j_k)$and check whether all empty cells are still reachable from the forest entrance.

If they are not, cancel the placement.

Stop the process once the number of placed trees reaches $K$.
</p>

<p>
Finally, choose the coordinates of the legendary flower $(t_i, t_j)$uniformly at random from the empty cells that satisfy the required conditions.
</p>

</section>

</div>

<div>

<section>

### **Tools (Input generator, local tester, and visualizer)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc054/YDAxDRZr_v2.html?lang=en">Web version</a>: This is more powerful than the local version providing animations.
</li>

<li>
<a href="https://img.atcoder.jp/ahc054/YDAxDRZr_v2.zip">Local version</a>: You need a compilation environment of <a href="https://www.rust-lang.org/">Rust language</a>.
<ul>

<li>
<a href="https://img.atcoder.jp/ahc054/YDAxDRZr_v2_windows.zip">Pre-compiled binary for Windows</a>: If you are not familiar with the Rust language environment, please use this instead.
</li>

</ul>

</li>

</ul>

<p>
Please be aware that sharing visualization results or discussing solutions/ideas during the contest is prohibited.
</p>

#### **Input File Format Used by the Tool**

<p>
The input file used for the local tester follows the format below:
</p>

<div>

$N$$t_i$$t_j$$b_{0,0}\cdots b_{0,N-1}$$\vdots$$b_{N-1,0}\cdots b_{N-1,N-1}$$q_i^0$$q_j^0$$\vdots$$q_i^{N^2-2}$$q_j^{N^2-2}$
</div>

<p>
The entries $(q_i^k, q_j^k)$appended at the end represent the $k$-th destination candidates.

When the adventurer chooses a destination, the list is traversed in this order, and the first cell that satisfies the conditions is selected.

The list $q$is generated by shuffling the $N^2 - 1$cells excluding the forest entrance in a random order.
</p>

</section>

</div>

<div>

<section>

### **Sample Solution (Python)**

<details>
A sample solution in Python is shown below.  
This program keeps track of the revealed cells but does not place any Treants.


```
N, ti, tj = map(int, input().split())
b = [input() for _ in range(N)]
revealed = [[False] * N for _ in range(N)]
while True:
    pi, pj = map(int, input().split())
    parts = input().split()
    n = int(parts[0])
    xy = list(map(int, parts[1:]))
    for k in range(n):
        x = xy[2 * k]
        y = xy[2 * k + 1]
        revealed[x][y] = True
    if pi == ti and pj == tj:
        break
    print(0, flush=True)
```

</details>

</section>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

20 16 8
........T..T........
..............T.....
T...................
........T...........
...T................
.....T..............
..........T.........
....................
......T.T.........T.
....T..........T..T.
.T..T........T.....T
........T...........
....................
.....TT.............
.................T..
....................
..........T.........
............T.....T.
....................
...........T.TTT....
16 3
1 7
8 6
8 13
3 1
13 2
16 6
2 5
18 10
10 9
19 2
7 10
6 12
4 7
10 4
10 7
18 8
12 2
14 2
3 7
4 19
14 7
18 5
5 4
4 2
14 16
11 4
0 3
0 0
8 18
19 17
11 5
18 17
18 12
10 1
8 7
17 3
16 18
16 15
0 5
13 13
14 1
8 9
19 10
17 4
15 9
9 11
1 16
4 1
10 5
1 14
17 7
17 10
11 10
8 5
6 9
4 5
4 3
12 9
6 2
4 17
8 2
19 19
12 1
2 4
8 10
13 7
5 16
2 17
5 0
16 0
14 10
6 13
18 13
12 7
0 12
11 9
8 15
10 18
11 11
16 11
5 12
9 15
7 13
15 1
16 9
7 9
15 10
1 13
7 16
7 18
3 10
1 2
18 1
15 11
5 8
6 16
8 12
2 3
18 14
5 14
13 10
2 9
17 12
0 4
11 3
13 6
17 16
14 4
16 5
14 15
17 1
16 8
3 11
12 11
8 19
1 5
5 7
12 16
0 2
17 0
19 8
7 11
10 2
3 6
0 16
5 1
4 16
19 9
7 6
3 9
6 11
16 2
13 3
19 15
12 13
6 10
6 7
16 12
15 7
13 18
8 14
19 7
4 18
15 14
11 13
4 12
11 16
17 8
2 14
12 19
15 5
9 19
12 5
13 19
3 13
9 16
10 17
7 14
3 0
6 5
17 19
9 17
15 2
1 17
17 6
2 13
9 8
5 19
9 2
8 8
15 16
15 12
15 4
10 6
4 8
7 19
10 19
18 9
9 0
10 12
16 4
15 17
1 12
18 0
13 16
14 5
9 5
13 9
1 11
2 0
14 12
14 14
2 12
7 8
1 18
5 13
9 9
10 13
16 16
3 4
17 5
0 7
5 3
17 2
11 12
13 17
18 3
1 19
1 1
6 17
12 6
15 0
8 3
11 17
8 1
14 0
15 8
7 3
14 19
2 15
15 18
17 14
2 6
3 3
12 3
10 16
6 8
3 8
14 9
10 14
18 18
3 15
0 15
11 15
18 16
5 15
3 17
16 19
11 6
5 2
13 8
12 15
5 10
6 0
7 0
5 5
4 10
7 17
11 8
6 1
4 6
19 11
7 5
10 15
18 2
18 11
2 1
12 0
0 9
5 18
13 14
15 6
9 18
9 3
15 15
4 11
2 2
13 0
8 0
9 6
9 12
9 13
9 7
5 6
4 14
12 17
2 19
2 18
14 17
8 11
6 18
3 14
5 17
11 19
1 3
15 3
10 11
18 6
19 4
17 9
14 11
19 18
17 15
0 13
11 14
3 19
7 7
4 15
9 1
12 10
2 11
19 16
9 14
4 0
6 14
10 0
17 17
12 4
17 13
16 10
13 1
2 7
19 6
12 12
0 11
7 12
19 13
0 6
12 8
19 1
14 13
1 6
11 1
0 1
0 18
7 1
14 8
6 19
4 4
1 15
8 17
5 11
5 9
16 14
10 3
13 15
0 14
1 10
7 4
3 2
3 5
6 6
6 4
3 16
12 14
15 13
18 4
19 12
17 11
15 19
6 15
13 4
16 7
4 13
7 2
19 3
12 18
1 0
16 17
10 8
11 18
8 4
18 7
6 3
19 0
19 14
16 1
16 13
1 4
1 8
0 19
18 15
2 10
0 17
14 18
7 15
1 9
9 4
14 3
11 0
14 6
13 11
3 12
11 2
2 8
4 9
3 18
8 16
19 5
2 16
11 7
13 5
17 18
13 12
10 10
0 8
9 10
18 19

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1 1 10
0 
1 1 8
2 2 8 2 10
-1

</div>

</section>

</div>

</span>

</span>

</div>
