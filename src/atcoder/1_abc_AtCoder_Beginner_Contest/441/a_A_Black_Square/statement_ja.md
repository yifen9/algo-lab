
<div>

<span>

<span>

<p>
配点 : $100$点
</p>

<div>

<section>

### **問題文**

<p>
$10^{100}$行 $10^{100}$列のマス目があります。

以下では、上から $i$行目かつ左から $j$列目のマスをマス $(i,j)$と表します。
</p>

<p>
マス目のうち、マス $(P,Q)$を一番左上のマスとした $100\times 100$マスの領域のみが黒く塗られており、それ以外のマスは白く塗られています。

マス $(X,Y)$が黒く塗られているか判定してください。  
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq P,Q,X,Y \leq 10000$
</li>

<li>
$P,Q,X,Y$は整数
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

$P$$Q$$X$$Y$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
マス $(X,Y)$が黒く塗られているならば `Yes`を、そうでないならば `No`を出力せよ。
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
5 10

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Yes

</div>

<p>
マス $(3,3)$を最も左上のマスとする $100\times 100$マスの領域が黒く塗られています。

マス $(5,10)$はこの領域に含まれているため、`Yes`を出力します。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5 5
10 1000

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

No

</div>

<p>
マス $(5,5)$を最も左上のマスとする $100\times 100$マスの領域が黒く塗られています。

マス $(10,1000)$はこの領域に含まれていないため、`No`を出力します。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

1 2
1 1

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

No

</div>

<p>
マス $(1,2)$を最も左上のマスとする $100\times 100$マスの領域が黒く塗られています。

マス $(1,1)$はこの領域に含まれていないため、`No`を出力します。
</p>

</section>

</div>

</span>

</span>

</div>
