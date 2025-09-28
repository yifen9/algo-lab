
<div>

<span>

<span>

<p>
配点 : $1700$点
</p>

<div>

<section>

### **問題文**

<p>
この世界には $1$から $K(=4)$までの番号がついた $K$種類の宝石があります．
種類 $i$の宝石の大きさ $1$あたりの価値は $W_i$です．
</p>

<p>
すぬけくんは $N$個の宝石を持っています．
$i$番目の宝石は種類 $A_i$で，大きさ $B_i$です．
また，すぬけくんは $N$個の箱を持っており，$i$番目の箱は大きさ $i$です．
</p>

<p>
すぬけくんは今から，それぞれの箱に宝石を $1$つずつ入れます．
宝石の大きさが箱より大きいときは，箱に入るように宝石を削ります．
つまり，宝石 $i$を箱 $j$に入れると，その価値は $W_{A_i} \times \min(B_i,j)$になります．
</p>

<p>
宝石の価値の総和としてありうる最大値を求めてください．
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>

<span>
$K=4$
</span>

</li>

<li>
$1 \leq W_1 < W_2 < \cdots < W_K \leq 10^6$
</li>

<li>
$1 \leq N \leq 250000$
</li>

<li>
$1 \leq A_i \leq K$
</li>

<li>
$1 \leq B_i \leq N$
</li>

<li>
入力はすべて整数である
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

$N$$K$$W_1$$W_2$$\ldots$$W_K$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_N$$B_N$
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

3 4
1 2 3 4
4 2
1 3
3 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

15

</div>

<p>
宝石 $1,2,3$をそれぞれ箱 $3,1,2$に入れると，価値の総和は $4 \times \min(2,3)+1 \times \min(3,1)+3 \times \min(2,2)=15$となり，これが最大です．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3 4
1 2 3 4
3 1
2 2
1 3

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

10

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

6 4
1 3 8 10
2 2
1 4
2 2
3 1
3 4
4 3

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

86

</div>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

15 4
239277 249169 419371 744281
2 14
1 4
1 11
4 12
1 7
2 12
3 15
2 5
3 4
1 8
3 2
4 1
1 15
3 5
2 8

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

39858078

</div>

</section>

</div>

</span>

</span>

</div>
