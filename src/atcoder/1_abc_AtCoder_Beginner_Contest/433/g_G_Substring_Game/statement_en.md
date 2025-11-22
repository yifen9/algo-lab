
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
You are given a string $S$consisting of lowercase English letters.
</p>

<p>
Alice and Bob play the following game using this string.
</p>

<ul>

<li>
Prepare an empty string $T$.
</li>

<li>
Starting with Alice, they take turns playing.
</li>

<li>
On each turn, the player chooses one lowercase English letter and concatenates the chosen letter to the end of $T$. Here, the player cannot take an action such that $T$after concatenation is not a substring of $S$.
</li>

</ul>

<p>
The player who cannot make a move first loses.
</p>

<p>
Determine which player will win when both players play optimally.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le T\le 10^5$
</li>

<li>
$T$is an integer.
</li>

<li>
$S$is a string consisting of lowercase English letters with length between $1$and $2\times 10^5$, inclusive.
</li>

<li>
The sum of the lengths of $S$over all test cases is at most $4\times 10^5$.
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case is given in the following format.
</p>

<div>

$S$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for the test cases in order, separated by newlines.
</p>

<p>
For each test case, output `Alice`if Alice wins when both players play optimally, and `Bob`if Bob wins.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4
ooxo
abrakadabra
atcoderbeginnercontest
baabca

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Bob
Alice
Alice
Bob

</div>

<p>
Consider the first test case.
</p>

<p>
For example, the game proceeds as follows.
</p>

<ul>

<li>
Alice chooses `x`. $T=$`x`.
</li>

<li>
Bob chooses `o`. $T=$`xo`.
</li>

<li>
No matter which lowercase English letter Alice chooses and concatenates to the end of $T$, $T$will not be a substring of $S$, so Alice cannot make a move. At this point, Bob wins.
</li>

</ul>

<p>
In this test case, Bob can win no matter how Alice plays. Therefore, output `Bob`.
</p>

</section>

</div>

</span>

</span>

</div>
