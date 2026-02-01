
<div>

<span>

<span>

<div>

<section>

### **Story**

<p>
In the Kingdom of Nihonbashi, there are many "ice cream trees." Two flavors are famous here: Traditional Vanilla and Passionate Strawberry.
People in this country value the variety of flavor combinations more than the total amount of ice cream.
</p>

<p>
The kingdom is a graph with vertices and edges. These vertices represent either ice cream trees or ice cream shops.
As an ice cream maker, you move around this graph, harvest flavors from trees to stack them on your cone, and deliver the completed ice cream to the shops.
</p>

<p>
A shop's satisfaction is determined by the diversity of its inventory — how many different flavor combinations it has.
Right now, all shops are empty. Your mission is to maximize the total satisfaction of all ice cream shops to make the kingdom lively again.
</p>

</section>

</div>

<div>

<section>

### **Problem Statement**

<p>
There is a connected undirected graph with $N$vertices and $M$edges. The vertices are numbered $0, 1, \ldots, N-1$. The $i$-th edge connects vertex $A_i$and vertex $B_i$.
</p>

<p>
Each vertex is one of the following two types:
</p>

<ul>

<li>
Ice Cream Shops: Vertices $0, 1, \ldots, K-1$($K$vertices in total).
</li>

<li>
Ice Cream Trees: Vertices $K, K+1, \ldots, N-1$($N-K$vertices in total).
</li>

</ul>

<p>
Each ice cream tree provides a specific flavor: Vanilla (`W`= White) or Strawberry (`R`= Red). Initially, all ice cream trees provide Vanilla (`W`).
</p>

<p>
You start at vertex $0$(an ice cream shop) with an empty cone (represented by an empty string). You can perform up to $T$steps. In each step, choose one of the following two actions:
</p>

<ul>

<li>
Action 1: Move from your current vertex to an adjacent vertex $v$. Then, depending on the type of $v$, either harvest ice cream or make a delivery.
<ul>

<li>
If $v$is an ice cream tree: Harvest the current flavor (`W`or `R`) from that tree and add it to the end of your cone's string.
</li>

<li>
If $v$is an ice cream shop: Add the current flavor string on your cone to the shop's inventory set $S_v$. Then, your cone becomes empty. You may deliver an empty string; in this case, the empty string is added to the inventory set $S_v$.
</li>

<li>

<strong>
Restriction: You cannot move back to the vertex you just came from in your previous Action 1
</strong>
. Specifically, if your last Action 1 was moving from vertex $a$to vertex $b$, your next Action 1 cannot be moving from $b$back to $a$(even if you performed Action 2 in between).
</li>

</ul>

</li>

<li>
Action 2: This action can only be performed if your current position is a Vanilla (`W`) ice cream tree. By adding strawberry juice, the flavor harvested from this tree changes to Strawberry (`R`) for all future harvests. You cannot change a Strawberry tree back to Vanilla.
</li>

</ul>

<p>
As described in the Input Generation, the graph is 2-edge-connected, so Action 1 is always possible.
</p>

<p>
Maximize the size of the inventory set $S_v$for each ice cream shop $v$.
Note that delivering a string that is already in $S_v$does not increase the size of the set.
</p>

</section>

</div>

<div>

<section>

### **Scoring**

<p>
Your score is the sum of the sizes of the inventory sets $S_i$across all ice cream shops $i$($0 \le i \lt K$): $\sum_{i=0}^{K-1} |S_i|$
</p>

<p>
If the following invalid outputs are produced, it will be judged as 
<span>
WA
</span>
.
</p>

<ul>

<li>
You perform Action 2 when your current vertex is not a Vanilla (`W`) ice cream tree.
</li>

<li>
In Action 1, you specify a vertex that is not directly connected to your current vertex by an edge.
</li>

<li>
In Action 1 (from the second time onwards), you move to the vertex from which you departed in the previous Action 1.
</li>

<li>
The total number of actions exceeds $T$.
</li>

</ul>

<p>
There are 150 test cases, and the score of a submission is the total score for each test case.
If your submission produces an illegal output or exceeds the time limit for some test cases, the submission itself will be judged as 
<span>
WA
</span>
or 
<span>
TLE
</span>
, and the score of the submission will be zero.
The highest score obtained during the contest will determine the final ranking, and there will be no system test after the contest. If more than one participant gets the same score, they will be ranked in the same place regardless of the submission time.
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

$N$$M$$K$$T$$A_{0}$$B_{0}$$\vdots$$A_{M-1}$$B_{M-1}$$X_{0}$$Y_{0}$$\vdots$$X_{N-1}$$Y_{N-1}$
</div>

<ul>

<li>
The first line contains four integers $N$, $M$, $K$, $T$. These represent the number of vertices, the number of edges, the number of ice cream shops, and the maximum number of actions, respectively. These values satisfy $N = 100$, $K = 10$, and $T = 10000$. For the value of $M$, please refer to the "Input Generation" section.
</li>

<li>
The following $M$lines provide information about the edges. Edge $i$bi-directionally connects vertex $A_i$and vertex $B_i$.
</li>

<li>
The following $N$lines provide the coordinates $(X_i,Y_i)$of each vertex $i$used during input generation. These coordinates are integers satisfying $0 \leq X_i, Y_i \leq 300$and $(X_i, Y_i) \neq (X_j, Y_j)$for any $i \neq j$.  You may skip reading them if you don't need them.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$or fewer lines in the following format:
</p>

<ul>

<li>
To perform Action 1: Output the vertex index $v$of the destination.
</li>

</ul>

<div>

$v$
</div>

<ul>

<li>
To perform Action 2: Output `-1`.
</li>

</ul>

<div>

-1

</div>

<p>
<a href="https://img.atcoder.jp/ahc060/wX0NuJxV.html?lang=en&seed=0&output=sample">Show example</a>
</p>

</section>

</div>

<div>

<section>

### **Input Generation**

<p>
Let $\mathrm{rand}(L,U)$be a function that generates a uniform random integer between $L$and $U$, inclusive.
</p>

<ol>

<li>
For each vertex $i$, the coordinates $(X_i,Y_i)$are chosen as $X_i = \mathrm{rand}(0, 300)$, $Y_i = \mathrm{rand}(0, 300)$. If the Euclidean distance to any already generated vertex is $20$or less, the coordinates are re-selected. This process is repeated $N$times to obtain the vertex set $V$.
</li>

<li>
Compute the <a href="https://en.wikipedia.org/wiki/Delaunay_triangulation">Delaunay Triangulation</a>for the vertex set $V$, and let the resulting set of edges be $E$.
</li>

<li>
Randomly shuffle the edges of $E$, and perform the following operation on each edge in order:
<ul>

<li>
If removing the edge keeps the graph $(V,E)$2-edge-connected and free of articulation points, the edge is removed from $E$with a probability of $0.7$.
</li>

</ul>

</li>

<li>
The set $E$after processing all edges becomes the edge set of the graph.
</li>

</ol>

</section>

</div>

<div>

<section>

### **Tools (Input generator and visualizer)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc060/wX0NuJxV.html?lang=en">Web version</a>: This is more powerful than the local version, providing animations.
</li>

<li>
<a href="https://img.atcoder.jp/ahc060/wX0NuJxV.zip">Local version</a>: You need a compilation environment of <a href="https://www.rust-lang.org/">Rust language</a>.
<ul>

<li>
<a href="https://img.atcoder.jp/ahc060/wX0NuJxV_windows.zip">Pre-compiled binary for Windows</a>: If you are not familiar with the Rust language environment, please use this instead.
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

</span>

</span>

</div>
