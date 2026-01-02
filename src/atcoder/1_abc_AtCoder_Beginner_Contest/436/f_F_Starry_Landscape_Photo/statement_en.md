
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
In the night sky seen from planet AtCoder, there are $N$stars, and these $N$stars are arranged in a line from east to west.
The $i$-th star from the east $(1\le i\le N)$is the $B _ i$-th brightest among these stars.
</p>

<p>
Takahashi decided to take a picture of the night sky using the following procedure:
</p>

<ol>

<li>
Choose a pair of integers $(l,r)$satisfying $1\le l\le r\le N$, and set up the camera so that the $l$-th, $(l+1)$-th, $\ldots$, $r$-th stars from the east all fit in the frame, and no other stars enter the frame.
</li>

<li>
Choose an integer $b$satisfying $1\le b\le N$, and open the shutter so that all stars among the $N$stars whose brightness ranks from $1$st through $b$-th (and that fit in the frame) are captured, and no other stars are captured.
</li>

</ol>

<p>
However, he may not take a picture with no stars captured.
</p>

<p>
Find the number of different sets of stars that can be captured in pictures taken in this way.
</p>

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
$1\le B _ i\le N\ (1\le i\le N)$
</li>

<li>
$B _ i\ne B _ j\ (1\le i\lt j\le N)$
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

$N$$B _ 1$$B _ 2$$\ldots$$B _ N$
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

4
3 1 4 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

12

</div>

<p>
For example, with $(l,r)=(2,4),b=3$, you can take a picture with two stars: the $2$nd star from the east and the $4$th star from the east.
</p>

<p>
Including this, you can take pictures with the following $12$different sets of stars.
In each picture, stars further east are arranged further left, and the $i$-th brightest star is labeled with integer $i$.
</p>

<p>

<img src="https://img.atcoder.jp/abc436/58d5efe8a68a28a223364b9040cb8561.png">

</img>

</p>

<p>
No other sets can be captured, so print `12`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

7
1 2 3 4 5 6 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

28

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

20
15 5 13 17 9 11 20 4 14 16 6 3 8 19 12 7 10 18 2 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

627

</div>

</section>

</div>

</span>

</span>

</div>
