
<div>

<span>

<span>

<p>
Score : $700$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a string $S$consisting of `(`and `)`.
</p>

<p>
Taro and Jiro will play the following game using this string.
</p>

<p>
Taro goes first and Jiro goes second; they alternately choose and perform one of the following three types of operations:
</p>

<ul>

<li>
Delete the first character of $S$.
</li>

<li>
Delete the last character of $S$.
</li>

<li>
Declare termination.
</li>

</ul>

<p>
The game ends when the length of $S$becomes exactly $K$, or when either player declares termination. At the end of the game, if $S$is a correct bracket sequence, Jiro wins; otherwise, Taro wins.
</p>

<p>
Given $S$before the game starts, determine the winner when both players act optimally.
</p>

<p>
You are given $T$test cases. Solve each of them.
</p>

<details>

<summary>
What is a correct bracket sequence?
</summary>
A correct bracket sequence is a string that can be reduced to an empty string by repeating the operation of deleting a substring `()`zero or more times.


</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 10^5$
</li>

<li>
$1 \le K < |S| \le 10^6$
</li>

<li>
$S$is a string consisting of `(`and `)`.
</li>

<li>
$T$and $K$are integers.
</li>

<li>
The sum of $|S|$over all test cases is at most $10^6$.
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

$T$$case_1$$case_2$$\vdots$$case_T$
</div>

<p>
Each case is given in the following format:
</p>

<div>

$S$$K$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
For each test case, print `First`if Taro wins, and `Second`if Jiro wins.
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
(()())
2
(())()
2
(()
2
(()()())((()()(())()))
12

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Second
First
First
First

</div>

<p>
For the first test case, here is an example of how the game might proceed:
</p>

<ul>

<li>

<p>
Before the game starts, $S$is `(()())`.
</p>

</li>

<li>

<p>
Taro deletes the first character of $S$, resulting in `()())`.
</p>

</li>

<li>

<p>
Next, Jiro deletes the last character of $S$, resulting in `()()`.
</p>

</li>

<li>

<p>
Next, Taro deletes the last character of $S$, resulting in `()(`.
</p>

</li>

<li>

<p>
Next, Jiro deletes the last character of $S$, resulting in `()`, and the length of $S$becomes $K=2$, so the game ends.
</p>

</li>

<li>

<p>
The final $S$is a correct bracket sequence, so Jiro wins.
</p>

</li>

</ul>

<p>
In the third test case, for example, Taro can win by declaring termination on the first turn.
</p>

</section>

</div>

</span>

</span>

</div>
