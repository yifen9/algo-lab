
<div>

<span>

<span>

<p>
配点 : $575$点
</p>

<div>

<section>

### **問題文**

<p>
$N$個の英小文字からなる文字列 $S_1,S_2,\dots,S_N$が与えられます。
</p>

<p>
$(1,2,\dots,N)$の順列 $P=(P_1,P_2,\dots,P_N)$としてありえるもの全てについて、以下の通りに生成される文字列を書き並べます。
</p>

<ul>

<li>
$S_{P_1},S_{P_2},\dots,S_{P_N}$をこの順に連結する。
</li>

</ul>

<p>
書き並べられた $N!$個の文字列を辞書順に並べた列を $A_1,A_2,\dots,A_{N!}$とします。

$A_2$を出力してください。
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
$1 \le T \le 1.5 \times 10^5$
</li>

<li>
$2 \le N \le 3 \times 10^5$
</li>

<li>
$T,N$は整数
</li>

<li>
$S_i$は英小文字からなる長さ $1$以上 $10^6-1$以下の文字列
</li>

<li>
ひとつの入力について、 $N$の総和は $3 \times 10^5$を超えない
</li>

<li>
ひとつの入力について、全てのテストケースにおける $|S_i|$の総和は $10^6$を超えない
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

$\text{case}_i$は $i$番目のテストケースを表す。
</p>

<div>

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる。
</p>

<div>

$N$$S_1$$S_2$$\vdots$$S_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力せよ。
</p>

<p>
$i$行目には $i$番目のテストケースについて、答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3
3
abc
ac
ahc
4
aaa
a
aaaa
a
15
ks
sy
k
ysk
yks
ky
ksy
sk
syk
s
kys
sky
ys
yk
y

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

abcahcac
aaaaaaaaa
kksksykykysskskyssyksyyksykyskyys

</div>

<p>
この入力には $3$個のテストケースが含まれています。
</p>

<p>
$1$番目のテストケースについて、 $S=($`abc`, `ac`, `ahc`$)$です。

$A=($`abcacahc`, `abcahcac`, `acabcahc`, `acahcabc`, `ahcabcac`, `ahcacabc`$)$なので、 $A_2=$`abcahcac`を出力します。
</p>

</section>

</div>

</span>

</span>

</div>
