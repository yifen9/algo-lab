
<div>

<span>

<span>

<p>
配点 : $250$点
</p>

<div>

<section>

### **問題文**

<p>
$N$行 $N$列からなるグリッドがあります。グリッドの上から $i$行目左から $j$列目のマスは、$S_{i,j}$が `#`のとき黒く、`.`のとき白く塗られています。
</p>

<p>
このグリッドから縦 $M$行横 $M$列の領域を取り出して得られるマスの塗られ方は何種類ありますか？
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq M \leq N \leq 10$
</li>

<li>
$N,M$は整数
</li>

<li>
$S_{i,j}$は `.`または `#`
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

$N$$M$$S_{1,1}\ldots S_{1,N}$$\vdots$$S_{N,1}\ldots S_{N,N}$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3 2
...
###
#.#

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3

</div>

<p>
与えられたグリッドの状態は下図左のとおりです。

ここから縦 $2$行横 $2$列の領域を取り出す方法は下図右のとおり $4$通りあり、マスの塗られ方は $3$種類あります。
</p>

<p>

<img src="https://img.atcoder.jp/abc430/f9240b594bb2c8463ffca0c0f7ec1b40.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

10 3
..#.......
.###......
.#.#......
#####.....
#...#.....
......####
......#..#
......#...
......#..#
......####

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

36

</div>

</section>

</div>

</span>

</span>

</div>
