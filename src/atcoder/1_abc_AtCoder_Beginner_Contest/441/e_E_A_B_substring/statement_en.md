
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a string $S$of length $N$consisting of three kinds of characters: `A`, `B`, and `C`.
</p>

<p>
There are $\dfrac{N(N+1)}2$non-empty contiguous substrings of $S$. Find how many of them contain more `A`s than `B`s.
</p>

<p>
Note that two substrings are counted separately if they are taken from different positions in $S$, even if they are equal as strings.
</p>

<details>

<summary>
What is a substring?
</summary>

<p>
A 
<strong>
substring
</strong>
of $S$is a string obtained by deleting zero or more characters from the beginning and zero or more characters from the end of $S$.

For example, `AB`is a substring of `ABC`, but `AC`is not a substring of `ABC`.
</p>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le5\times10 ^ 5$
</li>

<li>
$S$is a string of length $N$consisting of `A`, `B`, and `C`.
</li>

<li>
$N$is an integer.
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

$N$$S$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the number of contiguous substrings of $S$that contain more `A`s than `B`s.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

10
ACBBCABCAB

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

8

</div>

<p>
The following eight substrings satisfy the condition:
</p>

<ul>

<li>
`A`: 1st to 1st character of $S$
</li>

<li>
`AC`: 1st to 2nd character of $S$
</li>

<li>
`CA`: 5th to 6th character of $S$
</li>

<li>
`CABCA`: 5th to 9th character of $S$
</li>

<li>
`A`: 6th to 6th character of $S$
</li>

<li>
`ABCA`: 6th to 9th character of $S$
</li>

<li>
`CA`: 8th to 9th character of $S$
</li>

<li>
`A`: 9th to 9th character of $S$
</li>

</ul>

<p>
All other substrings do not satisfy the condition, so print `8`.
</p>

<p>
Note that `A`and `CA`can be taken from multiple positions, but they are counted separately if taken from different positions.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4
CCBC

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

<p>
There may be no substrings that satisfy the condition.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

36
CABACBBBBBAABABACCBCABCCABAABABBCBAC

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

136

</div>

</section>

</div>

</span>

</span>

</div>
