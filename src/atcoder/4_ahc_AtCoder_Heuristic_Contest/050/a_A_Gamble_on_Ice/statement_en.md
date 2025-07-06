
<div>

<span>

<span>

<div>

<section>

### **Problem Statement**

<p>
There is a skating rink consisting of an $N \times N$grid. The top-left cell has coordinates $(0,0)$, and a cell located $i$cells downward and $j$cells to the right has coordinates $(i,j)$. The area outside the $N \times N$grid is entirely covered by rocks and cannot be entered. Initially, $M$cells contain rocks.
</p>

<p>
Using this skating rink and a single robot, you play the following game:
</p>

<ul>

<li>
At the beginning of the game, your prize money is 0 yen.
</li>

<li>
First, you declare a sequence $P = ( P_0,P_1,\dots,P_{N^2 - M - 1} )$, which is an arbitrary ordering of the $N^2 - M$rock-free cells.
</li>

<li>
Then, one of the rock-free cells is uniformly randomly selected, and the robot is placed there.
</li>

<li>
Afterwards, for $i = 0,1,\dots,N^2 - M - 1$, the following is repeated:
<ul>

<li>
First, the robot uniformly randomly selects one of the four directions: up, down, left, or right.
</li>

<li>
Then, the robot moves in that direction in a straight line until it hits a rock.
<ul>

<li>
Note that the robot may not move at all.
</li>

</ul>

</li>

<li>
After that, a rock is placed on cell $P_i$.
<ul>

<li>
If the robot is on that cell, it is crushed and the game ends.
</li>

<li>
If the robot is not on that cell, you earn 1 yen.
</li>

</ul>

</li>

</ul>

</li>

</ul>

<p>
Find a sequence $P$that maximizes the expected value of the total prize money you can earn.
</p>

</section>

</div>

<div>

<section>

### **Scoring**

<p>
Let $E$be the expected value of the total prize money you can earn. Then, your score is $\displaystyle {\rm round} \left ( \frac{10^6 \times E}{N^2 - M - 1} \right )$.
</p>

<p>
There are $150$test cases, and the score of a submission is the total score for each test case.
If your submission produces an illegal output or exceeds the time limit for some test cases, the submission itself will be judged as 
<span>
WA
</span>
or 
<span>
TLE
</span>
, and the score of the submission will be zero.
The highest score obtained during the contest will determine the final ranking, and there will be no system test after the contest.
If more than one participant gets the same score, they will be ranked in the same place regardless of the submission time.
</p>

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

$N$$M$$S_{0,0} \dots S_{0,N-1}$$\vdots$$S_{N-1,0} \dots S_{N-1,N-1}$
</div>

<ul>

<li>
In all test cases, $N$is fixed to $40$.
</li>

<li>
$M$is an integer between $N^2/10$and $N^2/4$, inclusive.
</li>

<li>
Each $S_{i,0} \dots S_{i,N-1}$is a string of $N$characters consisting of `#`and `.`, where `#`indicates that cell $(i,j)$initially contains a rock, and `.`indicates that cell $(i,j)$is initially rock-free.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let the computed sequence $P$be represented as $P_i=(x_i,y_i)$. Output it to Standard Output in the following format:
</p>

<div>

$x_0$$y_0$$\vdots$$x_{N^2 - M - 1}$$y_{N^2 - M - 1}$
</div>

<p>
The sequence $P$must satisfy the following constraints:
</p>

<ul>

<li>
All $P_i$must be distinct.
</li>

<li>
For every $P_i$, the corresponding cell must be rock-free in the initial state.
</li>

</ul>

<p>
<a href="https://img.atcoder.jp/ahc050/k1BmZE1o.html?lang=en&seed=0&output=sample">Show example</a>
</p>

</section>

</div>

<div>

<section>

### **Input Generation**

<ul>

<li>
First, set $N=40$.
</li>

<li>
Next, choose an integer $M$uniformly at random from the range $N^2/10$to $N^2/4$, inclusive.
</li>

<li>
Finally, select $M$distinct cells uniformly at random from the $N^2$cells, and place rocks on those cells to determine the initial state of the grid.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Tools (Input generator and visualizer)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc050/k1BmZE1o.html?lang=en">Web version</a>: This is more powerful than the local version providing animations and manual play.
</li>

<li>
<a href="https://img.atcoder.jp/ahc050/k1BmZE1o.zip">Local version</a>: You need a compilation environment of <a href="https://www.rust-lang.org/">Rust language</a>.
<ul>

<li>
<a href="https://img.atcoder.jp/ahc050/k1BmZE1o_windows.zip">Pre-compiled binary for Windows</a>: If you are not familiar with the Rust language environment, please use this instead.
</li>

</ul>

</li>

</ul>

<p>
Please be aware that sharing visualization results or discussing solutions/ideas during the contest is prohibited.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

40 282
.#......#..#.#..........................
............#..............#..##...#..#.
......#........##..#...##......#.#......
.##..#...#......#.#.#....#....##.#....#.
............#..............#.......#.#..
..#.....#.....#...##......#............#
......#.....#......#.#.....##..#.##..#..
#.#.#.....#.#.#....#.#..........#.......
#...##.......#...#...#.......#....#.....
#..#...#...#....#...#........#...#.#....
....#..........#.......#..#.............
...##.......#.#..........#.#..........#.
..#.......#.....#.#..#.........#..##....
..##..##....#.............#.........#...
............................#...........
...#...#....#..####.#...........#.......
.##..........#.#.#..................#...
#...#.##............#......##..#........
............#.#...#...#.#..#..#....#....
......#.#........................#.###.#
....##......#..............#.#..........
#....#...#......#.#....#....#.......##..
..#......#......#.#............##..#....
....#.............#..#.#............#..#
.....#......#..##.....#....###.....#.#..
#...#...#.#.....#.....................#.
#........#.......#..........#.....###...
....#..#........#.......#...#.##.##..#..
#..........##.#.#.#....#......#.#..##...
.....##.....#....#..#.................#.
...#...#...#......##.....#..........#..#
.....#..#.................##............
..#.............##...#.......##.........
...#.#.........#.......................#
..#...#..#...................#...#......
.........#.....................#..#.....
#...##..#...............#.#....##.#.##..
#..#.........#...............##...#....#
#................#.......#.......#..#.#.
...#...#....#........#.........###....##

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

17 17
7 15
21 20
18 1
19 13
5 13
2 21
4 31
31 31
17 21
31 13
24 36
9 28
6 14
14 13
12 20
18 28
11 20
12 3
11 16
18 4
31 25
29 29
19 38
12 9
33 21
36 1
20 34
33 36
39 6
36 14
32 34
32 8
31 12
25 17
38 5
36 23
22 39
24 25
34 28
31 34
35 19
1 15
18 2
21 39
32 10
4 7
20 9
34 16
27 18
11 0
32 4
27 0
21 17
30 6
0 27
18 6
1 13
23 13
18 33
29 16
7 35
24 24
3 13
11 37
10 35
20 19
11 5
35 5
38 4
2 38
31 2
0 37
29 32
38 24
9 39
32 24
5 12
38 20
7 30
34 39
13 13
0 15
34 10
17 18
13 14
12 33
35 12
10 9
21 29
14 9
29 2
14 2
22 15
18 26
38 6
27 36
13 35
3 15
37 32
5 5
36 25
20 8
33 10
26 22
2 10
26 3
39 8
15 24
21 15
37 14
11 26
17 14
33 1
39 2
35 27
22 14
2 30
8 38
19 20
31 10
31 4
39 29
12 24
2 0
2 17
28 21
0 4
19 10
17 10
2 32
18 16
34 30
22 11
10 28
17 24
9 12
37 8
33 35
14 6
35 10
35 29
10 31
26 7
10 17
33 28
20 20
4 14
22 21
27 12
13 18
37 1
5 25
7 22
34 13
13 4
37 18
33 2
18 8
4 13
30 1
33 16
0 22
33 0
22 3
35 11
17 26
12 17
22 25
17 12
34 0
29 0
21 34
39 34
8 6
24 23
7 28
35 3
31 21
11 11
22 4
5 10
29 13
1 4
22 12
31 39
26 33
8 23
25 5
33 7
7 16
22 36
11 22
37 20
9 34
4 34
20 35
5 11
10 6
0 24
21 2
3 27
12 38
17 8
32 5
28 2
39 16
14 26
1 6
29 37
8 14
5 35
24 4
18 25
3 39
33 18
39 1
35 30
14 24
15 10
30 21
33 25
33 14
17 3
30 22
26 12
16 12
1 11
34 5
37 24
3 14
16 5
20 32
0 39
27 20
17 11
32 25
22 34
8 39
30 38
34 17
20 10
38 22
36 12
39 5
4 33
15 30
6 7
31 36
12 1
15 4
36 30
23 35
3 10
12 26
1 29
35 20
5 9
16 32
4 32
10 21
29 24
28 6
38 32
29 8
15 21
14 25
13 38
35 7
9 2
20 15
32 31
11 30
6 11
25 3
20 13
10 10
7 11
23 32
35 0
27 22
12 6
20 38
3 3
34 19
8 31
19 24
9 6
5 16
9 1
4 11
6 1
21 32
39 19
29 19
23 9
25 25
24 18
31 11
38 23
10 2
39 0
16 37
5 33
4 15
16 27
20 26
5 20
37 25
4 38
10 33
4 22
15 29
34 37
9 23
30 8
26 15
39 14
25 20
16 14
9 27
28 24
14 8
8 20
14 31
34 34
13 19
27 6
36 2
29 4
35 33
19 30
28 20
22 10
2 12
26 5
38 35
11 28
2 34
8 37
21 7
18 23
1 25
25 33
9 13
10 29
0 9
10 39
36 39
22 26
13 8
23 19
27 35
24 34
33 17
24 2
10 18
21 8
31 9
27 2
29 11
0 29
8 36
4 39
30 31
15 38
9 9
3 23
17 1
11 24
13 9
11 7
25 31
23 12
6 25
21 35
13 39
33 33
34 7
10 22
0 6
22 6
26 13
37 5
13 15
22 8
4 1
1 14
11 17
12 37
16 25
32 14
12 19
16 8
6 18
22 28
28 37
11 34
8 26
19 31
37 26
8 12
3 4
29 23
17 34
14 38
14 29
21 19
20 25
1 23
13 27
11 19
17 22
7 9
1 33
38 34
1 20
27 9
38 8
14 35
28 39
22 7
30 32
15 8
18 34
6 20
6 8
35 26
2 14
16 34
35 18
1 24
35 4
12 0
27 19
39 28
2 18
1 17
22 24
17 36
10 13
20 36
10 20
4 16
35 25
32 33
18 11
26 23
3 22
14 23
2 36
8 8
34 15
11 23
38 10
38 29
4 2
38 30
39 4
0 10
36 17
8 35
37 7
5 34
20 7
14 32
8 3
29 9
28 19
27 26
29 10
7 33
12 25
8 16
18 36
38 2
7 31
36 7
32 20
15 6
0 32
20 37
14 12
5 3
3 32
38 14
37 21
31 16
6 38
7 37
24 31
17 15
32 19
16 26
34 1
34 3
10 12
35 21
11 10
25 22
26 18
19 17
14 7
18 31
39 25
30 29
31 33
10 19
4 25
32 39
38 1
29 35
34 24
5 27
24 10
27 8
35 32
39 17
12 28
35 2
30 24
22 38
19 22
26 11
13 25
38 12
22 30
30 27
17 2
32 35
0 17
16 33
30 23
32 0
14 1
4 17
19 15
2 7
19 29
38 3
26 2
6 10
25 14
31 19
2 22
12 23
31 7
23 8
14 10
7 24
13 22
33 34
33 27
21 4
36 27
37 22
19 32
34 31
16 38
28 29
21 10
38 21
3 12
28 25
27 15
34 18
24 21
39 20
37 2
25 39
39 35
31 35
39 37
33 29
37 35
36 9
22 37
4 19
14 14
20 17
8 2
10 32
29 7
29 18
30 33
32 6
21 22
39 10
32 3
10 14
7 7
10 8
34 25
37 15
0 16
36 19
36 33
12 15
36 15
12 32
5 30
1 5
4 36
25 28
37 28
5 36
27 23
38 39
1 7
20 24
19 4
8 15
9 25
0 34
36 21
6 30
36 3
35 24
26 10
5 29
36 16
35 1
4 18
30 20
37 38
14 19
15 0
1 28
12 39
13 31
1 39
38 18
8 24
29 3
4 30
31 38
8 11
0 28
1 32
3 21
2 35
28 5
9 24
0 3
31 23
17 38
12 4
1 2
4 6
7 13
26 14
10 25
2 13
21 11
39 23
34 21
33 19
1 22
12 27
21 38
11 2
29 14
19 19
6 32
28 13
18 15
22 17
18 3
17 39
2 8
25 36
29 22
9 5
31 14
29 30
1 21
0 18
36 38
16 7
31 37
23 0
38 9
11 18
35 6
14 15
14 33
27 11
12 11
23 1
13 24
1 18
4 9
36 11
7 25
11 33
35 28
26 16
37 31
29 39
13 1
30 10
15 2
21 12
34 38
36 20
3 17
6 17
13 17
33 4
23 28
14 37
31 24
12 5
30 5
9 22
4 29
9 17
1 1
16 10
25 35
18 17
35 13
19 26
5 21
12 7
17 25
37 12
6 16
0 0
31 28
5 32
4 21
8 1
25 11
16 29
0 21
27 32
9 30
3 36
23 3
15 25
38 13
5 7
32 27
15 34
2 39
17 30
32 28
19 2
16 18
34 12
0 23
1 16
31 17
19 7
20 33
31 29
28 7
24 11
38 28
16 3
0 5
25 32
37 23
37 11
24 32
32 7
2 25
25 26
19 1
3 8
26 19
25 29
11 6
5 31
24 0
6 4
21 33
26 1
31 6
32 15
29 27
18 10
13 23
11 8
32 12
15 9
18 39
15 35
10 30
0 7
7 5
39 9
28 27
25 6
5 0
30 16
19 14
14 0
34 8
24 14
34 32
30 26
25 23
13 30
17 35
19 11
10 11
28 34
29 31
31 1
3 11
39 15
19 5
25 19
29 21
15 37
15 26
39 24
36 10
31 22
14 5
24 33
30 0
16 24
20 14
30 30
33 24
31 15
2 37
23 31
38 15
28 15
25 1
22 29
23 14
24 9
5 6
14 22
13 37
34 22
3 28
9 10
33 11
16 30
24 6
35 8
19 21
6 39
33 6
11 29
3 24
10 7
27 17
39 11
8 18
11 13
5 22
18 19
12 22
14 16
38 27
3 7
14 17
25 7
33 23
10 34
26 25
21 30
20 11
23 33
29 15
19 9
21 26
33 13
3 26
23 25
23 34
26 24
36 6
8 22
39 36
37 16
28 8
32 9
30 28
25 37
21 25
0 30
3 37
23 30
25 9
27 38
21 1
27 1
24 1
38 31
6 5
4 3
33 31
32 22
5 15
29 34
33 30
22 0
25 2
26 30
37 37
23 10
3 35
33 22
14 34
32 26
17 19
38 19
6 36
33 26
33 9
36 29
36 22
0 14
7 20
12 8
24 8
38 7
20 0
26 38
25 21
6 3
0 2
2 1
32 13
12 13
30 15
17 29
24 39
25 24
18 21
13 29
26 21
18 7
13 34
11 9
6 9
2 20
30 13
13 20
0 38
8 33
18 32
10 3
22 5
24 38
31 30
17 9
18 38
6 15
38 26
17 5
15 28
26 20
37 6
4 4
20 3
14 27
31 20
7 38
27 13
21 3
7 17
0 20
23 37
23 17
30 12
5 37
6 22
33 20
3 6
0 35
23 7
13 10
29 36
4 26
20 21
20 23
39 18
7 8
11 32
11 36
15 1
3 34
13 16
32 36
25 15
11 31
7 29
9 37
32 11
23 38
19 25
26 31
10 38
23 2
15 27
19 12
4 23
0 33
1 19
32 1
16 22
5 17
21 31
9 18
35 35
36 28
4 24
6 29
27 29
37 33
21 24
18 5
30 2
16 0
24 26
33 12
16 4
2 2
30 34
13 32
5 23
22 1
28 33
26 26
28 9
30 35
10 37
2 11
26 37
34 26
6 13
7 36
12 14
26 32
12 30
27 3
0 12
23 27
39 22
4 8
21 21
23 24
15 14
20 1
39 26
9 38
18 29
23 5
8 19
9 31
0 25
21 13
1 8
17 13
16 9
21 14
35 14
6 23
31 0
9 14
16 28
37 4
1 37
37 9
11 21
28 10
9 19
21 27
26 29
35 16
24 30
29 1
7 18
22 13
27 27
13 5
15 31
34 23
28 31
15 11
28 26
1 10
6 26
17 23
14 18
32 32
7 27
36 13
14 4
28 22
18 37
6 0
8 30
15 5
33 37
31 3
13 0
0 26
37 17
32 18
38 37
11 15
19 23
4 5
33 38
37 19
34 36
22 22
39 27
26 4
34 35
9 36
10 24
7 23
30 17
23 26
16 23
28 17
27 14
0 31
31 18
3 0
23 15
8 27
10 16
7 6
35 37
1 0
7 39
14 20
8 10
37 27
9 21
34 11
30 37
15 22
14 11
39 30
9 26
2 26
18 13
29 33
24 19
25 34
19 3
20 6
36 18
15 36
10 36
2 9
13 21
13 28
12 12
23 16
33 32
28 28
16 35
29 28
25 27
4 28
38 11
7 34
27 25
7 1
18 9
35 39
29 25
5 38
8 28
17 33
24 20
22 20
15 33
8 25
14 3
15 13
12 36
31 32
20 30
10 1
22 33
11 35
18 0
28 38
17 16
35 38
27 5
27 21
19 28
22 19
16 19
25 12
4 20
15 19
30 4
34 4
7 3
5 1
24 7
23 11
26 8
2 4
16 11
0 36
2 29
34 27
32 38
24 17
39 13
20 2
22 23
6 2
25 18
19 16
0 19
13 11
14 30
32 23
18 20
35 23
30 9
34 20
6 35
10 0
20 22
6 24
20 39
28 3
28 1
19 18
10 5
26 6
4 10
33 8
7 26
35 15
19 34
23 6
9 15
8 32
16 39
5 4
16 6
32 37
35 17
27 10
1 26
8 7
15 39
16 21
36 35
19 27
16 16
14 36
2 3
5 24
14 21
17 32
35 36
3 29
38 16
28 4
26 39
4 0
19 0
9 8
23 22
26 27
13 33
11 1
25 30
15 23
9 4
1 9
1 36
2 5
34 14
37 36
24 13
1 3
23 29
29 26
30 14
16 20
17 37
21 6
24 3
20 28
35 22
27 39
20 16
10 27
5 28
12 29
20 18
23 20
14 39
37 10
8 9
16 31
1 34
22 27
11 39
2 27
9 32
3 19
25 13
2 28
20 31

</div>

</section>

</div>

</span>

</span>

</div>
