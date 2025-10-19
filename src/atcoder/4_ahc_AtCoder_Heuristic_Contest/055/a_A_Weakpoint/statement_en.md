
<div>

<div>

<span>

<span>

<div>

<section>

### **Story**

<p>
"Nihonbashi Treasure Island" is a hugely popular novel in the fictional country R, and you are a big fan of the game based on this novel. In this game, numerous treasure boxes appear. Opening a treasure box allows you to acquire a weapon, which you can use to gain an advantage in the game.
</p>

<p>
To open a treasure box, you must attack it using either your bare hands or a weapon. Having heard that a secret ending is unlocked by opening all the treasure boxes in the game, you decide to find a way to open all of them with the minimum number of attacks, hoping to see the ending as soon as possible.
</p>

### **Problem Statement**

<p>
There are $N$treasure boxes, and the $i$-th treasure box is called treasure box $i$$(0 \le i \lt N)$. The initial hardness of treasure box $i$is $H_i$. Treasure box $i$contains weapon $i$.
</p>

<p>
When the hardness of treasure box $i$is reduced to $0$or less, treasure box $i$opens, and weapon $i$becomes available. Weapons have durability, and the durability of weapon $i$is $C_i$.
</p>

<p>
You can attack a treasure box using either your bare hands or an available weapon.
</p>

<ul>

<li>
Attack with bare hands: When you attack treasure box $b$with your bare hands, the hardness of treasure box $b$is reduced by $1$. There is no limit to the number of bare-handed attacks.
</li>

<li>
Attack with a weapon: When you attack treasure box $b$with weapon $w$, the hardness of treasure box $b$is reduced by $A_{w,b}$, and the durability of weapon $w$decreases by $1$. When the durability of weapon $w$reaches $0$, it breaks and can no longer be used for attacks.
</li>

</ul>

<p>
Find a sequence of attacks to open all the treasure boxes with as few attacks as possible.
</p>

</section>

</div>

---

<div>

<section>

### **Scoring**

<p>
Your score is 
<span>
\( \sum_{i=0}^{N-1} H_i - T + 1 \)
</span>
, where $T$is the number of attacks performed to open all treasure boxes.
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
Attacking an already opened treasure box
</li>

<li>
Attacking with a weapon that is not yet available
</li>

<li>
Attacking with a weapon whose durability has reached $0$
</li>

<li>
Outputting an invalid weapon number or treasure box number
</li>

<li>
Leaving any unopened treasure boxes after all attacks are finished
</li>

</ul>

<p>

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
Input will be provided from Standard Input in the following format.
</p>

<div>

\(
N \\
H_0 ~ H_1 ~ \ldots ~ H_{N-1} \\
C_0 ~ C_1 ~ \ldots ~ C_{N-1} \\
A_{0,0} ~ A_{0,1} ~ \ldots ~ A_{0,N-1} \\
A_{1,0} ~ A_{1,1} ~ \ldots ~ A_{1,N-1} \\
\vdots \\
A_{N-1,0} ~ A_{N-1,1} ~ \ldots ~ A_{N-1,N-1}
\)

</div>

<ul>

<li>
$N$is the number of treasure boxes. It is fixed at $N = 200$in all test cases.
</li>

<li>
The second line contains $N$space-separated integers $H_0, H_1, \ldots, H_{N-1}$representing the initial hardness of the treasure boxes. The hardness of treasure box $i$is $H_i$, satisfying $100 \leq H_i \leq 500$.
</li>

<li>
The third line contains $N$space-separated integers $C_0, C_1, \ldots, C_{N-1}$representing the durability of the weapons. The durability of weapon $i$is $C_i$, satisfying $1 \leq C_i \leq 6$.
</li>

<li>
The following $N$lines each contains  $N$space-separated integers, $A_{i, j}$.
                                
<ul>

<li>
$A_{i,j}$represents the value by which the hardness of treasure box $j$is reduced when attacked with weapon $i$, satisfying $1 \leq A_{i,j} \leq 500$.
</li>

</ul>

</li>

</ul>

### **Output**

<p>
Let $T$be the total number of attacks on the treasure boxes. Output $T$lines.
</p>

<div>

\(
W_{0}~B_{0}\\
\vdots \\
W_{T-1} ~ B_{T-1}
\)

</div>

<p>
For each line, output the weapon index $W_i$used for the $i$-th attack and the treasure box index $B_i$being attacked, in that order, separated by a space. If the $i$-th attack was performed with bare hands, $W_i$should be output as `−1`.
</p>

<p>
<a href="https://img.atcoder.jp/ahc055/ys4u9l6aru.html?lang=en&output=sample">show example</a>
</p>

</section>

</div>

</div>

<div>

<section>

### **Input Generation**

<ul>

<li>
$\mathrm{rand}(L, U)$: Generates an integer uniformly at random between $L$and $U$, inclusive.
</li>

<li>
$\mathrm{rand\_double}(L, U)$: Generates a real number uniformly at random between $L$and $U$, inclusive.
</li>

</ul>

<p>
Generate $H_i$, $C_i$, and $A_{i,j}$$(0 \le i \lt N, 0 \le j \lt N)$independently, as follows:
</p>

<ul>

<li>
$H_i = \mathrm{rand}(100, 500)$
</li>

<li>
$C_i = \mathrm{rand}(1, 6)$
</li>

<li>
$A_{i,j} = \mathrm{round}(500.0 / \mathrm{rand\_double}(1.0, 500.0))$
</li>

</ul>

</section>

</div>

<div>

<section>

### **Tools (Input generator and visualizer)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc055/ys4u9l6aru.html?lang=en">Web version</a>: This is more powerful than the local version providing animations.
</li>

<li>
<a href="https://img.atcoder.jp/ahc055/ys4u9l6aru.zip">Local version</a>: You need a compilation environment of <a href="https://www.rust-lang.org/">Rust language</a>.
                            
<ul>

<li>
<a href="https://img.atcoder.jp/ahc055/ys4u9l6aru_windows.zip">Pre-compiled binary for Windows</a>: If you are not familiar with the Rust language environment, please use this instead.
</li>

</ul>

</li>

</ul>

<p>
Please be aware that sharing visualization results or discussing solutions/ideas during the contest is prohibited.
                    
</p>

</section>

</div>

</span>

</span>

</div>

</div>
