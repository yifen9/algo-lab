
<div>

<span>

<span>

<p>
配点 : $300$点
</p>

<div>

<section>

### **問題文**

<p>
AtCoder 社は時刻 $0$に始業し時刻 $T$に終業します。 時刻 $t$と時刻 $t+1$との間隔は $1$秒です。

高橋君は AtCoder 社の業務時間中に SNS の chokutter を以下の規則で見ます。  
</p>

<ul>

<li>
始業と同時に chokutter を開く。
</li>

<li>
青木君が高橋君のデスクの後ろを通りかかった瞬間に chokutter を開いていた場合、直ちに chokutter を閉じる。
</li>

<li>
高橋君は、 chokutter を時刻 $t$に閉じると、時刻 $t+100$に必ず chokutter を開く。
</li>

</ul>

<p>
始業から終業までに $N$回青木君が高橋君のデスクの後ろを通りかかっており、そのうち $i$回目は時刻 $A_i$でした。

始業から終業までに、高橋君は合計で何秒 chokutter を見ていましたか？

なお、 
<strong>
高橋君が chokutter を開いた瞬間に青木君がデスクの後ろを通りかかることはありませんでした。
</strong>

</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
入力は全て整数
</li>

<li>
$0 \le N \le 3 \times 10^5$
</li>

<li>
$1 \le A_1 < A_2 < \dots < A_N \le T \le 10^9$
</li>

<li>
高橋君が chokutter を開いた瞬間に青木君がデスクの後ろを通りかかることはない
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

$N$$T$$A_1$$A_2$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

5 700
100 150 300 350 700

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

500

</div>

<ul>

<li>
時刻 $0$に高橋君は chokutter を開きます。
</li>

<li>
時刻 $100$に青木君が高橋君のデスクの後ろを通りかり、高橋君は直ちに chokutter を閉じます。
</li>

<li>
時刻 $150$に青木君が高橋君のデスクの後ろを通りかりますが、高橋君はこの時点で chokutter を開いていません。
</li>

<li>
時刻 $200$に高橋君は再び chokutter を開きます。
</li>

<li>
時刻 $300$に青木君が高橋君のデスクの後ろを通りかり、高橋君は直ちに chokutter を閉じます。
</li>

<li>
時刻 $350$に青木君が高橋君のデスクの後ろを通りかりますが、高橋君はこの時点で chokutter を開いていません。
</li>

<li>
時刻 $400$に高橋君は再び chokutter を開きます。
</li>

<li>
時刻 $700$に青木君が高橋君のデスクの後ろを通りかり、高橋君は直ちに chokutter を閉じます。
</li>

</ul>

<p>
高橋君は、合計で $500$秒間 chokutter を見ていました。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

0 1000000000


</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1000000000

</div>

<p>
青木君が高橋君のデスクの後ろを通りかかることがない場合もあります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10 1234
395 424 588 745 773 863 910 958 1102 1195

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

734

</div>

</section>

</div>

</span>

</span>

</div>
