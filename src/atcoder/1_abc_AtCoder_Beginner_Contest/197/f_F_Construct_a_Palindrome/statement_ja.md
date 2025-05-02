
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
$N$頂点 $M$辺の、単純とは限らない連結な無向グラフがあります。

辺 $i$は頂点 $A_i$と頂点 $B_i$を結んでおり、文字 $C_i$が書かれています。

頂点 $1$から頂点 $N$へのパス (同じ辺や頂点を複数回通っても構わない) を $1$つ選び、通る辺に書かれている文字を順に並べて文字列を作ります。

この文字列が回文になることはあるかを判定し、あるならばそのような回文の長さとして考えられる最小値を求めてください。  
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2 \le N \le 1000$
</li>

<li>
$1 \le M \le 1000$
</li>

<li>
$1 \le A_i \le N$
</li>

<li>
$1 \le B_i \le N$
</li>

<li>
$C_i$は英小文字
</li>

<li>
与えられるグラフは連結である
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

$N$$M$$A_1$$B_1$$C_1$$A_2$$B_2$$C_2$$A_3$$B_3$$C_3$$\hspace{25pt} \vdots$$A_M$$B_M$$C_M$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
作る文字列が回文になることがあるならば、そのような回文の長さの最小値を、ないならば `-1`を出力せよ。  
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

8 8
1 2 a
2 3 b
1 3 c
3 4 b
4 5 a
5 6 c
6 7 b
7 8 a

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

10

</div>

<p>
辺 $1, 2, 3, 1, 2, 4, 5, 6, 7, 8$の順に通ると、出来上がる文字列は `abcabbacba`となり、回文となります。

これより短い回文を作ることはできないので、答えは $10$です。  
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4 5
1 1 a
1 2 a
2 3 a
3 4 b
4 4 a

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

5

</div>

<p>
辺 $2, 3, 4, 5, 5$の順に通ると `aabaa`という文字列を作ることができ、これは回文です。

同じ辺や頂点を複数回通っても構わないことに注意してください。  
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

3 4
1 1 a
1 2 a
2 3 b
3 3 b

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

-1

</div>

<p>
出来上がる文字列が回文となることはありません。  
</p>

</section>

</div>

</span>

</span>

</div>
