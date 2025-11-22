
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
英小文字からなる文字列 $S$が与えられます。
</p>

<p>
Alice と Bob がこの文字列を使って以下のようなゲームを行います。
</p>

<ul>

<li>
空文字列 $T$を用意する。
</li>

<li>
Alice から始めて両者は交互に手番をプレイする。
</li>

<li>
各手番では、プレイヤーは英小文字を一つ選び、 $T$の末尾に選んだ英小文字を連結させる。ただし、連結させた後の $T$が $S$の部分文字列とならないような行動を取ることはできない。
</li>

</ul>

<p>
先に手番をプレイできなくなったプレイヤーの負けです。
</p>

<p>
両者が最善を尽くしたとき、どちらのプレイヤーが勝つかを求めてください。
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
$1\le T\le 10^5$
</li>

<li>
$T$は整数
</li>

<li>
$S$は英小文字からなる長さ $1$以上 $2\times 10^5$以下の文字列
</li>

<li>
全てのテストケースにおける $S$の長さの総和は $4\times 10^5$以下
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
各テストケースに対する答えを順に改行区切りで出力せよ。
</p>

<p>
各テストケースについて、両者が最善を尽くしたとき Alice が勝つならば `Alice`を、Bob が勝つならば `Bob`を出力せよ。
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
ooxo
abrakadabra
atcoderbeginnercontest
baabca

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Bob
Alice
Alice
Bob

</div>

<p>
$1$番目のテストケースについて考えます。
</p>

<p>
例えば、ゲームは以下のように進行します。
</p>

<ul>

<li>
Alice が `x`を選ぶ。 $T=$`x`となる。
</li>

<li>
Bob が `o`を選ぶ。 $T=$`xo`となる。
</li>

<li>
Alice がどの英小文字を選んで $T$の末尾に連結しても $T$が $S$の部分文字列となることはないため、Alice は手番をプレイすることができない。この時点で Bob の勝ちとなる。
</li>

</ul>

<p>
このテストケースは Alice がどのように手番をプレイしても Bob が勝つことができます。したがって、 `Bob`を出力してください。
</p>

</section>

</div>

</span>

</span>

</div>
