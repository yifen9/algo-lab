
<div>

<span>

<span>

<p>
Score : $200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
The AtCoder country has two official languages: Takahashi-go and Aoki-go.
</p>

<p>
Both Takahashi-go and Aoki-go use some lowercase English letters to write words in those languages.
Takahashi-go uses only the characters contained in a string $S$of length $N$, and Aoki-go uses only the characters contained in a string $T$of length $M$.
</p>

<p>
You are given $Q$words $w _ 1,w _ 2,\ldots,w _ Q$that are in the official languages of the AtCoder country.
For each word, determine which of the following applies based on the characters contained in that word:
</p>

<ul>

<li>
It is confirmed to be a word in Takahashi-go
</li>

<li>
It is confirmed to be a word in Aoki-go
</li>

<li>
Neither can be determined
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le26$
</li>

<li>
$1\le M\le26$
</li>

<li>
$S$is a string of length $N$consisting of lowercase English letters.
</li>

<li>
The characters in $S$are arranged in alphabetical order.
</li>

<li>
All characters in $S$are distinct.
</li>

<li>
$T$is a string of length $M$consisting of lowercase English letters.
</li>

<li>
The characters in $T$are arranged in alphabetical order.
</li>

<li>
All characters in $T$are distinct.
</li>

<li>
$1\le Q\le100$
</li>

<li>
$w _ i$is a string of length at least $1$and at most $100$consisting of lowercase English letters. $(1\le i\le Q)$
</li>

<li>
$w _ i$is a word in Takahashi-go or Aoki-go. $(1\le i\le Q)$
</li>

<li>
$N,M,Q$are integers.
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

$N$$M$$S$$T$$Q$$w _ 1$$w _ 2$$\vdots$$w _ Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $Q$lines.
The $i$-th line should contain `Takahashi`if it is confirmed that $w _ i$is a word in Takahashi-go, `Aoki`if it is confirmed to be a word in Aoki-go, and `Unknown`if neither can be determined.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

6 5
ahikst
aikot
5
asahi
okita
kiai
hash
it

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Takahashi
Aoki
Unknown
Takahashi
Unknown

</div>

<p>
For example, all of `a`, `s`, `h`, `i`are used in Takahashi-go, and `h`is not used in Aoki-go, so it is confirmed that `asahi`is a word in Takahashi-go.
Thus, print `Takahashi`on the first line.
</p>

<p>
Both `i`and `t`are used in both Takahashi-go and Aoki-go, so it cannot be determined whether `it`is a word in Takahashi-go or Aoki-go.
Thus, print `Unknown`on the fifth line.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

7 6
ahiknst
ahikos
5
kioki
ohiki
tashi
nishi
kashi

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

Aoki
Aoki
Takahashi
Takahashi
Unknown

</div>

<p>
`o`is not used in Takahashi-go, so the first two words are confirmed to be words in Aoki-go.
Thus, print `Aoki`on the first and second lines.
</p>

<p>
`t`and `n`are not used in Aoki-go, so the following two words are confirmed to be words in Takahashi-go.
Thus, print `Takahashi`on the third and fourth lines.
</p>

<p>
For the first four words, there is a rule that words ending in `shi`are Takahashi-go, and words ending in `ki`are Aoki-go. However, all of `k`, `a`, `s`, `h`, `i`are used in both Takahashi-go and Aoki-go, so it is impossible to determine which language the word `kashi`belongs to based on the characters used.
Thus, print `Unknown`on the fifth line.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

13 11
defghiqsvwxyz
acejmoqrtwx
15
qhsqzhd
jcareec
wwqxqew
wxqxwex
jxxrtwa
trtqjxe
sqyggse
xxqwxew
xewwxxw
wwqxwex
xqqxqwq
qxxexxe
teqeroc
eeeqqee
vxdevyy

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

Takahashi
Aoki
Unknown
Unknown
Aoki
Aoki
Takahashi
Unknown
Unknown
Unknown
Unknown
Unknown
Aoki
Unknown
Takahashi

</div>

</section>

</div>

</span>

</span>

</div>
