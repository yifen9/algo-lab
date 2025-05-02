
<div>

<span>

<span>

<p>
Score : $1600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
A 
<i>
balancing network
</i>
is an abstract device built up of $N$wires, thought of as running from left to right,
and $M$
<i>
balancers
</i>
that connect pairs of wires. The wires are numbered from $1$to $N$from top to bottom,
and the balancers are numbered from $1$to $M$from left to right.
Balancer $i$connects wires $x_i$and $y_i$($x_i < y_i$).
</p>

<div>

<img src="https://img.atcoder.jp/agc041/pic1-small-2acea94b.png">

</img>

</div>

<p>
Each balancer must be in one of two states: 
<i>
up
</i>
or 
<i>
down
</i>
.
</p>

<p>
Consider a token that starts moving to the right along some wire at a point to the left of all balancers.
During the process, the token passes through each balancer exactly once.
Whenever the token encounters balancer $i$, the following happens:
</p>

<ul>

<li>
If the token is moving along wire $x_i$and balancer $i$is in the down state, the token moves down to wire $y_i$and continues moving to the right.
</li>

<li>
If the token is moving along wire $y_i$and balancer $i$is in the up state, the token moves up to wire $x_i$and continues moving to the right.
</li>

<li>
Otherwise, the token doesn't change the wire it's moving along.
</li>

</ul>

<p>
Let a state of the balancing network be a string of length $M$, describing the states of all balancers.
The $i$-th character is `^`if balancer $i$is in the up state, and `v`if balancer $i$is in the down state.
</p>

<p>
A state of the balancing network is called 
<i>
uniforming
</i>
if a wire $w$exists such that, regardless of the starting wire,
the token will always end up at wire $w$and run to infinity along it. Any other state is called 
<i>
non-uniforming
</i>
.
</p>

<p>
You are given an integer $T$($1 \le T \le 2$). Answer the following question:
</p>

<ul>

<li>
If $T = 1$, find any uniforming state of the network or determine that it doesn't exist.
</li>

<li>
If $T = 2$, find any non-uniforming state of the network or determine that it doesn't exist.
</li>

</ul>

<p>
Note that if you answer just one kind of questions correctly, you can get partial score.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 50000$
</li>

<li>
$1 \leq M \leq 100000$
</li>

<li>
$1 \leq T \leq 2$
</li>

<li>
$1 \leq x_i < y_i \leq N$
</li>

<li>
All input values are integers.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Partial Score**

<ul>

<li>
$800$points will be awarded for passing the testset satisfying $T = 1$.
</li>

<li>
$800$points will be awarded for passing the testset satisfying $T = 2$.
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

$N$$M$$T$$x_1$$y_1$$x_2$$y_2$$:$$x_M$$y_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print any uniforming state of the given network if $T = 1$, or any non-uniforming state if $T = 2$. If the required state doesn't exist, output `-1`.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 5 1
1 3
2 4
1 2
3 4
2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

^^^^^

</div>

<p>
This state is uniforming: regardless of the starting wire, the token ends up at wire $1$.
</p>

<div>

<img src="https://img.atcoder.jp/agc041/pic2-small-2acea94b.png">

</img>

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 5 2
1 3
2 4
1 2
3 4
2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

v^^^^

</div>

<p>
This state is non-uniforming: depending on the starting wire, the token might end up at wire $1$or wire $2$.
</p>

<div>

<img src="https://img.atcoder.jp/agc041/pic3final-small-2acea94b.png">

</img>

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

3 1 1
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

-1

</div>

<p>
A uniforming state doesn't exist.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

2 1 2
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

-1

</div>

<p>
A non-uniforming state doesn't exist.
</p>

</section>

</div>

</span>

</span>

</div>
