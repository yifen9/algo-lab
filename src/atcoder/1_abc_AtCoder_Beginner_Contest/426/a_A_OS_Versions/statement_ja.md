
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
ある OS のバージョンは古い順に "`Ocelot`", "`Serval`", "`Lynx`" です。

バージョン $X$がバージョン $Y$以降のバージョンであるか判定してください。

なお、バージョン $X$自身もバージョン $X$以降のバージョンであるものとします。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$X,Y$は "`Ocelot`", "`Serval`", "`Lynx`" のいずれか (引用符を含まない)
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

$X$$Y$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
バージョン $X$がバージョン $Y$以降のバージョンであれば `Yes`、そうでなければ `No`と出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

Serval Ocelot

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
バージョン `Serval`はバージョン `Ocelot`以降のバージョンです。そのため、 `Yes`と出力します。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

Serval Lynx

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
バージョン `Serval`はバージョン `Lynx`以降のバージョンではありません。そのため、 `No`と出力します。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

Ocelot Ocelot

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

Yes

</div>

<p>
バージョン `Ocelot`自身もバージョン `Ocelot`以降のバージョンです。そのため、 `Yes`と出力します。
</p>

</section>

</div>

</span>

</span>

</div>
