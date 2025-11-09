
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
英小文字からなる文字列 $s$に対し、$s$の部分文字列であって、偶数長の回文であるものの個数を $f(s)$で表します。より厳密には、$f(s)$は以下の条件を全て満たす整数 $l, r$の組の個数です。
</p>

<ul>

<li>
$1 \leq l \leq r \leq |s|$
</li>

<li>
$r - l + 1$は偶数
</li>

<li>
$s_l s_{l+1} \cdots s_{r}$は回文
</li>

</ul>

<p>
英小文字からなる文字列 $S$が与えられるので、$S$の文字を並べ替えて得られる文字列 $S'$のうち、$f(S')$が最小となるものを $1$つ出力してください。
</p>

<p>
$T$個のテストケースが与えられるので、それぞれについて解いてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \le T \le 10^5$
</li>

<li>
$2 \le |S| \le 2 \times 10^5$
</li>

<li>
$S$は英小文字からなる
</li>

<li>
全てのテストケースにおける $|S|$の総和は $2 \times 10^5$以下
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる。
</p>

<div>

$S$
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
$i$行目には $i$番目のテストケースについて、$S$の文字を並べ替えて得られる文字列 $S'$のうち、$f(S')$が最小となるものを $1$つ出力せよ。そのような $S'$が複数ある場合は、どれを出力しても正答となる。
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
see
xxxxxy
abracadabra

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

ese
xxxyxx
abracadabra

</div>

<p>
$1$番目のテストケースについて、$S$の文字を並べ替えて得られる文字列 $S'$として `see`, `ese`, `ees`が考えられますが、このうち $f(S')$が最小となるものは `ese`のみなので、これを出力します。
</p>

<p>
$2$番目のテストケースについて、例えば `xxyxxx`と出力しても正答となります。
</p>

</section>

</div>

</span>

</span>

</div>
