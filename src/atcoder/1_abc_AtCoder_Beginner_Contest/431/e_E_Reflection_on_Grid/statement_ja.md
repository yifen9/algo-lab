
<div>

<span>

<span>

<p>
配点 : ${500}$点
</p>

<div>

<section>

### **問題文**

<p>
$H$行 $W$列のマス目があります。 上から $i$行目、左から $j$列目のマスをマス $(i,j)$と呼ぶことにします。各マスには鏡が高々 $1$枚置いてあります。
</p>

<p>
高橋君はマス $(1,1)$の左側、青木くんはマス $(H,W)$の右側に立っています。高橋君は懐中電灯を持っており、マス $(1,1)$の左側から右に向かって光を入れています。ここで、懐中電灯の光は拡散せず、まっすぐに進む光線であるとします。
</p>

<p>
高橋君の目標は、マス目にある鏡を利用して懐中電灯の光を青木君に届けることです。
</p>

<p>
鏡の置き方は次の $3$種類あります。光が鏡に当たると、鏡の置き方に応じて光の進む向きが変わります。それぞれの鏡の置き方について、光が入る方向に対する出る方向は下図のようになります。
</p>

<ul>

<li>
タイプ A （鏡は置かれていない）
</li>

</ul>

<p>

<img src="https://img.atcoder.jp/abc431/9a3821cb76d936b95b6979e084d56994.png">

</img>

</p>

<ul>

<li>
タイプ B （左上と右下を結ぶ対角線上に鏡が置かれている）
</li>

</ul>

<p>

<img src="https://img.atcoder.jp/abc431/283ea6eabada389e76e89518fcb9fb18.png">

</img>

</p>

<ul>

<li>
タイプ C （右上と左下を結ぶ対角線上に鏡が置かれている）
</li>

</ul>

<p>

<img src="https://img.atcoder.jp/abc431/9410773fd7615321f27f070d5f0b1844.png">

</img>

</p>

<p>
マス目の鏡の置き方は $H$個の長さ $W$の文字列 $S_1,S_2,\ldots,S_H$で表されます。$S_i$の $j$文字目が `A`のときマス $(i,j)$はタイプ A、`B`のときマス $(i,j)$はタイプ B、`C`のときマス $(i,j)$はタイプ C です。
</p>

<p>
高橋君は、青木君に光を届けるために以下の操作を好きな回数行うことができます。
</p>

<ul>

<li>
あるマスを $1$つ選び、そのマスの鏡の置き方を別のタイプに変更する
</li>

</ul>

<p>
青木君に光を届けるためには最低何回操作を行う必要があるか求めてください。
</p>

<p>
$T$個のテストケースが与えられるので、それぞれについて答えを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq T$
</li>

<li>
$1\leq H,W$
</li>

<li>
$HW\leq 2\times 10^5$
</li>

<li>
$S_i$は `A`, `B`, `C`からなる長さ $W$の文字列
</li>

<li>
$T,H,W$は整数
</li>

<li>
全てのテストケースに対する $HW$の総和は $2\times 10^5$以下
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる。
</p>

<div>

$H$$W$$S_1$$S_2$$\vdots$$S_H$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力せよ。$i$行目には $i$番目のテストケースに対する答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4
3 4
ABCB
CACC
BCBA
2 2
CB
AA
1 10
BCBCBCBCBC
10 10
CCAABACAAA
CCCBACACCA
BACAABCBBA
ACCCAACCCA
CCAAAACCBA
AACBBACCAA
BCCCACBBAB
CBBCAACCCC
CBBCCBCBCA
BBACABBACC

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

0
2
10
5

</div>

<p>
$1$つ目のテストケースについて、操作を行わなくても青木君に光を届けることができます。
</p>

<p>

<img src="https://img.atcoder.jp/abc431/f66a190627b09b9e6c4cbacb84b6d9bd.png">

</img>

</p>

<p>
$2$つ目のテストケースについて、マス $(1,1)$の鏡の置き方をタイプ A に、マス $(2,2)$の鏡の置き方をタイプ B に変更することで、下図のように青木君に光を届けることができます。$1$回以下の操作で青木君に光を届けることはできないので、答えは $2$です。
</p>

<p>

<img src="https://img.atcoder.jp/abc431/1aeac5f2fecf4319d369b8cc3067959a.png">

</img>

</p>

</section>

</div>

</span>

</span>

</div>
