
<div>

<span>

<span>

<div>

<section>

### **Story**

<p>
In Japan, a traditional calligraphy contest known as 'Kakizome Taikai' is held during the New Year.
AtCoder's Kakizome Taikai is an event in which, instead of writing with a brush, each employee types on a keyboard with a special key layout and outputs his/her favorite string on a PC screen for presentation.
</p>

<p>
After learning many lucky words for this year through fortune-telling, CEO Takahashi decided to output a string containing all the lucky words as a (contiguous) substring (called a 
<strong>
lucky string
</strong>
).
For example, if the lucky words are `AC`, `WA`, and `CE`, then `WHITESPACE`is not a 
<strong>
lucky string
</strong>
because it does not contain `WA`as a substring, but `FACEWASH`is a 
<strong>
lucky string
</strong>
because it contains all lucky words as substrings.
</p>

<p>
Moving and typing a finger on the keyboard takes time depending on the distance between keys.
Because Takahashi is first in the order of presentation, he wants to type a 
<strong>
lucky string
</strong>
as quickly as possible.
Please help him by creating a program to determine how to move his finger.
</p>

</section>

</div>

<div>

<section>

### **Problem Statement**

<p>
You are given a key layout represented on an $N \times N$grid.
Let $(0, 0)$be the coordinates of the top-left square, and $(i, j)$be the coordinates of the square located $i$squares down and $j$squares to the right from there.
Each square contains an uppercase English letter $A_{i,j}$, and initially, the finger is placed on the square $(s_i, s_j)$.
</p>

<p>
You are given $M$strings $t_1,\cdots,t_M$consisting of uppercase English letters.
A string that contains all $t_k$as (contiguous) substrings is defined as a 
<strong>
lucky string
</strong>
.
Starting with an empty string $S$, the goal is to make $S$a 
<strong>
lucky string
</strong>
by performing the following operations no more than $5000$times.
</p>

<ul>

<li>
Specify square $(i, j)$, move the finger to this square, and then append $A_{i, j}$to the end of $S$. If the coordinates of the square where the finger was placed before the operation are $(i', j')$, this operation incurs a cost of $|i-i'|+|j-j'|+1$. The squares $(i, j)$and $(i', j')$can be the same, in which case the incurred cost is $1$.
</li>

</ul>

<p>
Find a sequence of operations that makes $S$a 
<strong>
lucky string
</strong>
with as little cost as possible.
</p>

</section>

</div>

<div>

<section>

### **Scoring**

<p>
Let $K$be the number of $t_k$contained in $S$as (contiguous) substrings, and $T$be the total cost of the operations.
Then you will obtain the following score.
</p>

<ul>

<li>
If $K\lt M$, $\mathrm{round}(1000 \times (K+1)/M)$.
</li>

<li>
If $K=M$, $\mathrm{max}(10000-T, 1001)$.
</li>

</ul>

<p>
If the number of operations exceeds $5000$, or if a square outside the $N\times N$grid is specified, it will be judged as 
<span>
WA
</span>
.
</p>

<p>
There are 150 test cases, and the score of a submission is the total score for each test case.
If your submission produces an illegal output or exceeds the time limit for some test cases, the submission itself will be judged as 
<span>
WA
</span>
or 
<span>
TLE
</span>
, and the score of the submission will be zero.
The highest score obtained during the contest will determine the final ranking, and there will be no system test after the contest.
If more than one participant gets the same score, they will be ranked in the same place regardless of the submission time.
</p>

</section>

</div>

---

<div>

<div>

<section>

### **Input**

<p>
Input is given from Standard Input in the following format:
</p>

<div>

$N$$M$$s_i$$s_j$$A_{0,0}$$A_{0,1}$$\cdots$$A_{0,N-1}$$A_{1,0}$$A_{1,1}$$\cdots$$A_{1,N-1}$$\vdots$$A_{N-1,0}$$A_{N-1,1}$$\cdots$$A_{N-1,N-1}$$t_1$$\vdots$$t_M$
</div>

<ul>

<li>
$N=15$
</li>

<li>
$M=200$
</li>

<li>
$0\le s_i,s_j\le N-1$
</li>

<li>
$A_{i,0}A_{i,1}\cdots A_{i,N-1}$is a string of length $N$consisting of uppercase English letters.
</li>

<li>
$t_k$is a string of length $5$consisting of uppercase English letters.
</li>

<li>
$t_k\ne t_{k'}$$(k\ne k')$
</li>

<li>
For every uppercase $c$, it is guaranteed that there exists at least one coordinate $(i,j)$such that $A_{i,j}=c$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $L$be the number of operations and $(i_l, j_l)$$(0\le i_l, j_l\le N-1)$be the square specified in the $l$-th operation.
Then, output to Standard Output in the following format.
</p>

<div>

$i_1$$j_1$$\vdots$$i_L$$j_L$
</div>

<p>
<a href="https://img.atcoder.jp/ahc028/fWRno7xB.html?lang=en&seed=0&output=sample">Show example</a>
</p>

</section>

</div>

<div>

<section>

### **Input Generation**

<p>

</p>

<details>
Let $\mathrm{rand}(L,U)$be a function that generates a uniform random integer between $L$and $U$, inclusive.
<p>

</p>

#### **Generation of $(s_i,s_j)$**

<p>
Generate $s_i=\mathrm{rand}(0, N-1)$and $s_j=\mathrm{rand}(0, N-1)$.
</p>

#### **Generation of $A_{i,j}$**

<p>
For each $(i, j)$, generate $A_{i,j}$uniformly at random from uppercase English letters.
If there exists an uppercase letter that is not included in any $A_{i,j}$, regenerate all $A_{i,j}$.
</p>

#### **Generation of $t_k$**

<p>
For each $k$, generate a string $t_k$of length $5$by randomly generating uppercase English letters $5$times.
If there is an already generated $t_{k'}$with $t_k=t_{k'}$, regenerate $t_k$.
Finally, sort $t_1, t_2, \cdots, t_M$in lexicographic order.
</p>

</details>

</section>

</div>

<div>

<section>

### **Tools (Input generator and visualizer)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc028/fWRno7xB.html?lang=en">Web version</a>: This is more powerful than the local version and can display animations.
</li>

<li>
<a href="https://img.atcoder.jp/ahc028/fWRno7xB.zip">Local version</a>: You need a compilation environment of <a href="https://www.rust-lang.org">Rust language</a>.
<ul>

<li>
<a href="https://img.atcoder.jp/ahc028/fWRno7xB_windows.zip">Pre-compiled binary for Windows</a>: If you are not familiar with the Rust language environment, please use this instead.
</li>

</ul>

</li>

</ul>

<p>
Please be aware that sharing visualization results or discussing solutions/ideas during the contest is prohibited.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

15 200
0 14
AWVECXNGDCNGBMQ
URGNCIDJOVTHSOB
KIGBCYVNJUYVRWC
EIXOMNZZLEBHWOX
DLPDTIFGWMQOMAQ
YSUDWSIOQRTBURH
DKTQGUCVOJIYSPP
SVLNHOOCDLDAMNF
JLFXHXINKYBVCGU
ESYKRPBSPYJIWZU
LRGACNSZRPKESVK
HDMSMPEBCXCTZTX
KMIXHCXJFZICBJX
TEGKFZOGIQLONVD
LVBIWLIHLAGARHI
ABYNP
AOTLX
ARZVJ
ASPBI
AXFSO
AZPGI
BCPZL
BENRS
BOVIS
BUBNT
BYUJQ
CBYSK
CINAP
CNCBN
COOUV
COPDO
CQQZD
DADKB
DGXFM
DLQFC
DQNCL
DRGYV
DSDUU
DWIZI
DZMWP
EBYAI
EKKOD
EKYQJ
EMLYM
EQLUL
ERGRD
ERWVW
ESLTA
FBGKH
FBPWX
FCTHA
FOIOY
FTPWX
FVJEJ
FYZVJ
GCSZE
GEBGT
GEPUH
GVLGE
GWTIL
GYEZT
HCGWP
HEQWH
HFXXC
HGWEW
HIPKG
HKHVZ
HUCSQ
HWNQT
HXIOS
IEOTI
IFMJA
IKFLQ
IKOTA
ILQFS
IQTXL
IRNAB
IXTRT
IZFIV
JBWWJ
JDYNL
JHWXZ
JKIRA
JNPBO
JODMD
JOWSW
JRMIO
JXUSI
JYCOD
JYKWU
KASYC
KDZPV
KRJKE
KVINZ
KZKQA
LEZYS
LHICS
LMLSY
LNUCX
MBPRA
MEAPP
MFJNA
MFRNF
MLXDV
MNQSF
MUSXF
MXRFN
MYGLL
NJGES
NQZTU
NRKRQ
NTAPK
NYOWZ
OAUQD
OKRRY
OMIAK
ONPWH
OUFYF
OXASM
OXSMM
PBAMY
PEJQR
PJFGR
PJXXR
PMQAC
PMXFC
POLAM
PPPAD
PRSKX
PSGLI
PUORC
PUUUP
PVNSO
PXUII
PZEPP
QDMII
QDXYM
QHHZU
QLNRU
QNDEH
QNWKI
QPCPS
QULFB
QVVVG
RGHTR
RGQWY
RHYGF
RIELA
RMAKH
ROVKG
RSSYP
RSULP
RWBAX
SICZS
SJBBE
SNCZK
SUMHS
SXEZH
SYXFA
TANTF
TDVIQ
TGMCV
THIWA
TLUET
TMAYP
TQCSB
TXYKE
UAQKR
UGHLN
UJKSD
ULGYC
UNUSS
UWNUQ
VBUYH
VCUMT
VIRUK
VMXTJ
VNVCN
VPBGX
WBWLB
WCNUF
WHAXY
WKAKT
WNMDP
WPHPJ
WULBH
WVFWE
WVYTO
WWCBS
WWUFL
XESTB
XHYES
XKDGD
XKHYZ
XMOJJ
XPCQR
XQEHC
XSOKS
XTGPA
XTLCE
XXSWV
XXVDA
YAPDH
YBDJA
YCNGF
YLDQD
YLFGP
YNBDS
YQGBT
YVJLV
YYPIT
ZBGGI
ZORJO
ZQMBO
ZYYVG

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1 13
2 14
4 10
5 8
3 7
4 3
6 1
7 3
9 4
8 8
5 9
4 10
8 11
8 11
10 13
14 10
13 10
10 9
9 14
8 14
9 14
6 13

</div>

</section>

</div>

</span>

</span>

</div>
