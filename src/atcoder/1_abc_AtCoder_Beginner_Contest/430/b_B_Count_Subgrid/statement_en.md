
<div>

<span>

<span>

<p>
Score : $250$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a grid with $N$rows and $N$columns. The cell at the $i$-th row from the top and $j$-th column from the left is painted black if $S_{i,j}$is `#`, and white if it is `.`.
</p>

<p>
How many distinct patterns of painted cells can be obtained by extracting a region of $M$rows and $M$columns from this grid?
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq M \leq N \leq 10$
</li>

<li>
$N$and $M$are integers.
</li>

<li>
$S_{i,j}$is `.`or `#`.
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

$N$$M$$S_{1,1}\ldots S_{1,N}$$\vdots$$S_{N,1}\ldots S_{N,N}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 2
...
###
#.#

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3

</div>

<p>
The state of the given grid is as shown in the left figure below.

There are four ways to extract a region of two rows and two columns from this grid as shown in the right figure below, and there are three distinct patterns of painted cells.
</p>

<p>

<img src="https://img.atcoder.jp/abc430/f9240b594bb2c8463ffca0c0f7ec1b40.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 3
..#.......
.###......
.#.#......
#####.....
#...#.....
......####
......#..#
......#...
......#..#
......####

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

36

</div>

</section>

</div>

</span>

</span>

</div>
