
<div>

<span>

<span>

<p>
配点 : $700$点
</p>

<div>

<section>

### **問題文**

<p>
$N$個のマスが横一列に並んでおり，左から順に $1$から $N$の番号がついています．
最初，すべてのマスは白色です．
</p>

<p>
あなたは以下の $M$種類の操作を
<strong>
好きな順序で好きな回数
</strong>
行うことができます．
</p>

<ul>

<li>
$i$種類目の操作: マス $L_i$からマス $R_i$までを黒色で塗る．
</li>

</ul>

<p>
マス目の状態を変化させるような操作の回数の最大値を求めてください．
なお，操作を行った結果色が変化したマスが $1$つでもあれば，その操作はマス目の状態を変化させたとみなします．
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 500$
</li>

<li>
$1 \leq M \leq N(N+1)/2$
</li>

<li>
$1 \leq L_i \leq R_i \leq N$
</li>

<li>
$(L_i,R_i) \neq (L_j,R_j)$($i \neq j$)
</li>

<li>
入力される値はすべて整数．
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
入力は以下の形式で標準入力から与えられる．
</p>

<div>

$N$$M$$L_1$$R_1$$L_2$$R_2$$\vdots$$L_M$$R_M$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを出力せよ．
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3 3
1 3
1 1
3 3

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
以下のように操作すると，マス目の状態を変化させる操作が $3$回行われます．
</p>

<ul>

<li>
$2$種類目の操作を行う．新たにマス $1$が黒色で塗られる．
</li>

<li>
$3$種類目の操作を行う．新たにマス $3$が黒色で塗られる．
</li>

<li>
$1$種類目の操作を行う．新たにマス $2$が黒色で塗られる．
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4 3
1 2
3 4
1 4

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

2

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

5 5
4 5
1 1
2 4
1 2
2 5

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

4

</div>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

20 15
2 4
16 19
7 13
1 15
3 18
10 11
1 10
1 7
14 16
1 16
2 17
1 17
12 14
3 17
4 10

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

11

</div>

</section>

</div>

</span>

</span>

</div>
