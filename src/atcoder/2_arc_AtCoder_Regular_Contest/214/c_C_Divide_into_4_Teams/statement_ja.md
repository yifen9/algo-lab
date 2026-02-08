
<div>

<span>

<span>

<p>
配点 : $600$点
</p>

<div>

<section>

### **問題文**

<p>
$1, \dots ,N$の番号がついた $N$人の人がいます。人 $i$の
<strong>
強さ
</strong>
は $P_i$です。
</p>

<p>
各人を $A,B,C,D$のいずれかのチームに割り当てることで、$4$つのチームにチーム分けをします。チーム分けの方法は $4^N$通りありますが、このうち以下の条件を全て満たすチーム分けの個数を $998244353$で割った余りを求めて下さい。
</p>

<ul>

<li>
$A,B,C,D$のどのチームにも $1$人以上所属する。
</li>

<li>
チーム $A$に所属する人の強さの和とチーム $B$に所属する人の強さの和が等しい。
</li>

<li>
チーム $C$に所属する人の強さの和とチーム $D$に所属する人の強さの和が等しい。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$4 \le N \le 500$
</li>

<li>
$1 \le P_i$
</li>

<li>
$\sum_{1 \le i \le N} P_i \le 10^5$
</li>

<li>
入力される値は全て整数
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

$N$$P_1$$P_2$$\ldots$$P_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
問題文中の条件を満たすチーム分けの個数を $998244353$で割った余りを出力せよ。
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
1 1 2 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

8

</div>

<p>
以下の $8$通りのチーム分けが条件を満たします。
</p>

<table>

<thead>

<tr>

<th>

</th>

<th>
人 $1$
</th>

<th>
人 $2$
</th>

<th>
人 $3$
</th>

<th>
人 $4$
</th>

</tr>

</thead>

<tbody>

<tr>

<td>
チーム分け $1$
</td>

<td>
A
</td>

<td>
B
</td>

<td>
C
</td>

<td>
D
</td>

</tr>

<tr>

<td>
チーム分け $2$
</td>

<td>
B
</td>

<td>
A
</td>

<td>
C
</td>

<td>
D
</td>

</tr>

<tr>

<td>
チーム分け $3$
</td>

<td>
A
</td>

<td>
B
</td>

<td>
D
</td>

<td>
C
</td>

</tr>

<tr>

<td>
チーム分け $4$
</td>

<td>
B
</td>

<td>
A
</td>

<td>
D
</td>

<td>
C
</td>

</tr>

<tr>

<td>
チーム分け $5$
</td>

<td>
C
</td>

<td>
D
</td>

<td>
A
</td>

<td>
B
</td>

</tr>

<tr>

<td>
チーム分け $6$
</td>

<td>
C
</td>

<td>
D
</td>

<td>
B
</td>

<td>
A
</td>

</tr>

<tr>

<td>
チーム分け $7$
</td>

<td>
D
</td>

<td>
C
</td>

<td>
A
</td>

<td>
B
</td>

</tr>

<tr>

<td>
チーム分け $8$
</td>

<td>
D
</td>

<td>
C
</td>

<td>
B
</td>

<td>
A
</td>

</tr>

</tbody>

</table>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

9
1 2 3 4 5 6 7 8 9

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

0

</div>

<p>
条件を満たすチーム分けが存在しません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

24
1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

289359125

</div>

</section>

</div>

</span>

</span>

</div>
