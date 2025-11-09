
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
For a string $s$consisting of lowercase English letters, let $f(s)$denote the number of substrings of $s$that are palindromes of even length. More precisely, $f(s)$is the number of pairs of integers $l, r$that satisfy all of the following conditions:
</p>

<ul>

<li>
$1 \leq l \leq r \leq |s|$.
</li>

<li>
$r - l + 1$is even.
</li>

<li>
$s_l s_{l+1} \cdots s_{r}$is a palindrome.
</li>

</ul>

<p>
Given a string $S$consisting of lowercase English letters, output one string $S'$obtained by rearranging the characters of $S$such that $f(S')$is minimized.
</p>

<p>
You are given $T$test cases. Solve each of them.
</p>

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
$2 \le |S| \le 2 \times 10^5$
</li>

<li>
$S$consists of lowercase English letters.
</li>

<li>
The sum of $|S|$over all test cases is at most $2 \times 10^5$.
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
Each test case is given in the following format:
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
Output $T$lines.
</p>

<p>
The $i$-th line should contain one string $S'$obtained by rearranging the characters of $S$in the $i$-th test case such that $f(S')$is minimized. If there are multiple such $S'$, any of them will be considered correct.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
see
xxxxxy
abracadabra

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

ese
xxxyxx
abracadabra

</div>

<p>
For the first test case, the strings $S'$obtained by rearranging the characters of $S$are `see`, `ese`, and `ees`. Among these, only `ese`minimizes $f(S')$, so output it.
</p>

<p>
For the second test case, for example, outputting `xxyxxx`will also be considered correct.
</p>

</section>

</div>

</span>

</span>

</div>
