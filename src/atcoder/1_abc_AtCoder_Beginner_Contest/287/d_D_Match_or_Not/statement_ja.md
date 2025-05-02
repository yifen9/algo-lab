
<div>

<span>

<span>

<p>
配点 : $400$点
</p>

<div>

<section>

### **問題文**

<p>
英小文字と `?`からなる文字列 $S,T$が与えられます。ここで、$|S| \gt |T|$が成り立ちます(文字列 $X$に対し、 $|X|$で $X$の長さを表します)。
</p>

<p>
また、$|X|=|Y|$を満たす文字列 $X,Y$は、次の条件を満たすとき及びそのときに限り
<strong>
マッチする
</strong>
といいます。
</p>

<ul>

<li>
$X,Y$に含まれる `?`をそれぞれ独立に好きな英小文字に置き換えることで $X$と $Y$を一致させることができる
</li>

</ul>

<p>
$x=0,1,\ldots,|T|$に対して次の問題を解いてください。
</p>

<ul>

<li>
$S$の先頭の $x$文字と末尾の $|T|-x$文字を順番を保ったまま連結することで得られる長さ $|T|$の文字列を $S'$とする。$S'$と $T$がマッチするならば `Yes`と、そうでなければ `No`と出力せよ。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$S,T$は英小文字と `?`からなる文字列
</li>

<li>
$1 \leq |T| \lt  |S| \leq 3 \times 10^5$
</li>

</ul>

</section>

</div>

---

<div>

<div>

<section>

### **入力**

<p>
入力は以下の形式で標準入力から与えられる。
</p>

<div>

$S$$T$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$|T|+1$行出力せよ。

$i$行目には $x=i-1$に対する出力をせよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

a?c
b?

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Yes
No
No

</div>

<p>
$x=0$の場合、$S'$は `?c`となります。ここで、$S'$の $1$文字目の `?`を `b`に、$T$の $2$文字目の `?`を `c`に置き換えることで $S'$と $T$を一致させることができるため、$S'$と $T$はマッチします。このため、$1$行目の出力は `Yes`です。

$x=1,2$の場合は $S'$はそれぞれ `ac`、`a?`であり、$T$とマッチしません。このため、$2,3$行目の出力は `No`です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

atcoder
?????

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

Yes
Yes
Yes
Yes
Yes
Yes

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

beginner
contest

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

No
No
No
No
No
No
No
No

</div>

</section>

</div>

</span>

</span>

</div>
