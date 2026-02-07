
<div>

<span>

<span>

<p>
配点 : $350$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の正整数列 $A=(A_1,A_2,\dots,A_N)$が与えられます。
</p>

<p>
以下のようなことが起こりうる正整数 $L$をすべて求めてください。
</p>

<blockquote>

<p>
AtCoder 社は棒状のスナック菓子「AtCoderりこ」を発売しました。
カップの中に長さ $L$の AtCoderりこが何本か入っています。
高橋君がこのカップをシェイクしたところ、それぞれの AtCoderりこは以下のいずれかの状態になりました。

</p>

<ul>

<li>
長さが $L$である $1$本の AtCoderりことしてそのまま残った。 
</li>

<li>
長さの和が $L$であるような $2$本の AtCoderりこに分かれた。ただし、各 AtCoderりこの長さは正整数である。
</li>

</ul>
カップをシェイクした後、カップの中には $N$本の AtCoderりこが入っており、$i$本目の AtCoderりこの長さは $A_i$でした。
<p>

</p>

</blockquote>

<p>
ただし、このようなことが起こりうる正整数 $L$が少なくとも $1$つ存在するような入力が与えられます。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 3 \times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^9$
</li>

<li>
条件を満たすような $L$が少なくとも $1$つ存在する
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

$N$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
条件を満たすような $L$を、空白区切りで昇順に $1$行で出力せよ。
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
10 5 5 10

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

10 15

</div>

<p>
最初、カップには長さ $10$の AtCoderりこが $3$本入っていて、そのうち $1$本が 長さ $5$の $2$本の AtCoderりこに分かれると、条件を満たします。

最初、カップには長さ $15$の AtCoderりこが $2$本入っていて、それぞれの AtCoderりこが長さ $5,10$の $2$本の AtCoderりこに分かれると、条件を満たします。

これ以外の $L$では条件を満たしません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3
4 4 4

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

4

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

6
10 187 344 100 434 257

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

444

</div>

</section>

</div>

</span>

</span>

</div>
