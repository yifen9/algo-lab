
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a directed graph with $N$vertices, vertex $1,$vertex $2,\ldots,$vertex $N$.
For any pair of integers $(i,j)$with $1 \leq i,j \leq N$, there is exactly one directed edge from vertex $i$to vertex $j$with cost $C_{i,j}$.
</p>

<p>
You are given a positive integer $K$.
For each of $s=1,2,\ldots,N$, solve the following problem.
</p>

<ul>

<li>
Among the ways to start at vertex $s$, move along an edge $K$times, and return to vertex $s$, find the minimum possible total cost of the edges traversed. More formally, find the minimum possible value of $\displaystyle\sum_{i=1}^{K}C_{v_{i-1},v_i}$for a sequence $v=(v_0,v_1,\ldots,v_K)$of integers between $1$and $N$, inclusive, of length $K+1$satisfying $v_0=v_K=s$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N \le 100$
</li>

<li>
$1 \le K \le 10^9$
</li>

<li>
$0 \le C_{i,j} \le 10^9\ (1 \le i \le N,1 \le j \le N)$
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

$N$$K$$C_{1,1}$$C_{1,2}$$\ldots$$C_{1,N}$$C_{2,1}$$C_{2,2}$$\ldots$$C_{2,N}$$\vdots$$C_{N,1}$$C_{N,2}$$\ldots$$C_{N,N}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines.
The $i$-th line $(1 \le i \le N)$should contain the answer to the problem for $s=i$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 3
3 1 4 1
5 9 2 6
5 3 5 8
9 7 9 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

8
8
8
9

</div>

<p>
For $s=1$, moving $1\rightarrow2\rightarrow3\rightarrow1$gives a total cost of $1+2+5=8$.
It is impossible to start at vertex $1$, move along an edge three times, and achieve a total cost of $7$or less, so print `8`on the first line.
</p>

<p>
For $s=4$, moving $4\rightarrow4\rightarrow4\rightarrow4$gives a total cost of $3+3+3=9$.
Note that the same edge or the same vertex may be traversed multiple times, and if the same edge is traversed multiple times, its cost is added to the total that many times.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 1000000000
100 999 999
999 100 999
999 999 100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

100000000000
100000000000
100000000000

</div>

<p>
The answer may be $2^{32}$or greater.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10 9482
748 169 586 329 972 529 432 519 408 587
138 249 656 114 632 299 984 755 404 772
155 506 832 854 353 465 387 374 567 385
631 556 951 428 104 705 530 406 258 102
709 325 334 193 520 798 749 582 337 910
530 110 659 635 786 773 811 468 810 638
111 822 554 627 395 959 924 698 777 893
142 848 532 781 711 814 665 395 960 290
746 266 603 553 893 353 323 640 172 263
749 921 845 334 594 821 233 695 109 951

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

1382481
1382481
1382628
1382481
1382481
1382540
1382481
1382739
1382499
1382481

</div>

</section>

</div>

</span>

</span>

</div>
