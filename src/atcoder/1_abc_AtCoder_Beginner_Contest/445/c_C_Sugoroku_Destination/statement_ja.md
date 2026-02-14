
<div>

<span>

<span>

<p>
配点 : $300$点
</p>

<div>

<section>

### **問題文**

<p>
マス $1,$マス $2,\ldots,$マス $N$の $N$個のマスが $1$列に並んでいます。
マス $i$には整数 $A _ i (i\le A_  i\le N)$が書かれています。
</p>

<p>
$s=1,2,\ldots,N$のそれぞれについて、以下の問題を解いてください。
</p>

<ul>

<li>
はじめ、マス $s$に駒を置く。「駒が置かれているマスに書かれている整数を $x$として、駒をマス $x$に移動させる」という操作を $10 ^ {100}$回行った後、駒が置かれているマスの番号を出力する。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N\le5\times10 ^ 5$
</li>

<li>
$i\le A _ i\le N\ (1\le i\le N)$
</li>

<li>
入力はすべて整数
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

$N$$A _ 1$$A _ 2$$\ldots$$A _ N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$s=1,2,\ldots,N$に対する答えを、この順に空白を区切りとして一行に出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

7
2 4 7 5 5 6 7

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

5 5 7 5 5 6 7

</div>

<p>
$s=1$のとき、駒は以下の図のように移動します。
</p>

<p>

<img src="https://img.atcoder.jp/abc445/c54c58fe4877e457dc58520027e2700f.png">

</img>

</p>

<p>
駒がマス $5$に置かれているとき、操作が行われても駒は移動しないため、$s=1$のときの答えは $5$となります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5
1 2 3 4 5

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1 2 3 4 5

</div>

<p>
駒が一度も移動しないこともあります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

15
11 3 10 7 15 10 10 11 11 13 11 12 14 14 15

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

11 14 14 14 15 14 14 11 11 14 11 12 14 14 15

</div>

</section>

</div>

</span>

</span>

</div>
