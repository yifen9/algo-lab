
<div>

<span>

<span>

<div>

<section>

### **ストーリー**

<p>
昔々、高橋王国にはたくさんの都市が点在していましたが、道路が無く人々は都市間の移動に苦労していました。
そこで国王の高橋くんは、都市をいくつかのグループに分け、グループ内の任意の2都市間が道路によって互いに行き来できるように都市を結ぶ道路を建設することで、国を発展させる計画を考えました。
高橋くんはなるべく建設する道路の総長を短くしたいと考えていましたが、高橋王国には正確な地図が無く、各都市の位置がはっきりしていないという問題がありました。
</p>

<p>
どのように道路を建設するべきか困った高橋くんは、王国一の占い師に助けを求めることにしました。
占い師は、いくつかの都市を選ぶことで、それらの都市同士を互いに行き来できるような総長の最も短い道路の建設方法を知ることができます。
ただし、占いの回数には限界があります。
</p>

<p>
なるべく建設する道路の総長を短くできるように、最適な占い方および道路の建設計画を考えてください。
</p>

</section>

</div>

<div>

<section>

### **問題文**

<p>
平面上に $N$個の都市があり、 $0$から $N-1$までの番号が付けられている。
都市 $i$の座標は $(x_i, y_i)$としてジャッジ内部では定まっているが、入力では与えられない。
その代わりに都市 $i$が存在する可能性のある座標の長方形範囲 $lx_i, rx_i, ly_i, ry_i$が与えられ、 $lx_i \le x_i \le rx_i$および $ly_i \le y_i \le ry_i$を満たす。
都市間の距離はユークリッド距離の小数点以下を切り捨てた整数値 $\mathrm{dist}(i, j) = \left\lfloor \sqrt{(x_i - x_j)^2 + (y_i - y_j)^2} \right\rfloor$として定義される。
</p>

<p>
長さ $M$の配列 $G$が与えられる。
各グループの大きさがそれぞれ $G_0, G_1, \dots, G_{M-1}$となるように都市を $M$個のグループに分割し、同じグループ内の都市が連結になるように道路を建設したい。
</p>

<p>
回答の出力を行う前に、占いとして以下の形式のクエリを最大 $Q$回まで行うことができる。
</p>

<ul>

<li>
都市の集合 $C \subset \{0,1,\cdots,N-1\}$を選ぶ。ただし、その大きさ $l = |C|$は、入力で指定される上限サイズ $L$に対して $2 \le l \le L$を満たす必要がある。
</li>

<li>
クエリに対する応答として、都市集合 $C$上での最小全域木を構成するための $l-1$本の道路それぞれが接続する都市の組が得られる。ここで、最小全域木は以下のアルゴリズムによって構築される。
<ul>

<li>
辺の配列 $E$を、都市集合 $C$に含まれる任意の 2 都市間の辺で初期化する。
</li>

<li>
$E$を都市間の距離の昇順にソートする。都市間の距離は都市の真の座標に基づいて計算される。都市間の距離が等しい辺については、辺が結ぶ2つの都市 $u<v$のペア $(u,v)$について昇順となるようにソートする。
</li>

<li>
$E$の先頭から順に辺を取り出し、その辺を追加したときに閉路ができないならば、その辺を最小全域木に追加する。
</li>

<li>
最小全域木を構成する各辺について、辺が結ぶ2つの都市 $u<v$のペア $(u,v)$について昇順にソートしたものをクエリに対する応答とする。
</li>

</ul>

</li>

</ul>

<p>
その後、以下を満たすような都市のグループ分けおよび道路の建設計画を出力せよ。
</p>

<ul>

<li>
$N$個の都市を $M$個のグループに分ける。各グループ $i$には $G_i$個の都市を割り当てる必要がある。いずれのグループにも割り当てられない都市や、複数のグループに割り当てられるような都市があってはならない。
</li>

<li>
各グループ $i$について、そのグループに属する都市間を結ぶ道路を $G_i - 1$本選ぶ。このとき、各グループ内の任意の2都市間が道路によって相互に到達可能、すなわちグラフとして連結となる必要がある。
</li>

</ul>

<p>
なお、それぞれの道路はその両端の 2 都市間のみを結ぶ。複数の道路が平面交差していても、道路から道路へ移ることはできない。
</p>

</section>

</div>

<div>

<section>

### **得点**

<p>
出力した道路の建設計画における全ての道路の総長が絶対スコアとなる。
都市 $i$と都市 $j$を結ぶ道路の長さは、真の座標を用いて計算された都市間の距離 $\mathrm{dist}(i, j) = \left\lfloor \sqrt{(x_i - x_j)^2 + (y_i - y_j)^2} \right\rfloor$として計算される。

<font color="red">
<strong>
絶対スコアは小さければ小さいほど良い。
</strong>
</font>

</p>

<p>
各テストケース毎に、 $\mathrm{round}(10^9 × \frac{全参加者中の最小絶対スコア}{自身の絶対スコア})$の
<font color="red">
<strong>
相対評価スコア
</strong>
</font>
が得られ、その和が提出の得点となる。
</p>

<p>
最終順位はコンテスト終了後に実施されるより多くの入力に対するシステムテストにおける得点で決定される。
暫定テスト、システムテストともに、一部のテストケースで不正な出力や制限時間超過をした場合、そのテストケースの相対評価スコアは0点となり、そのテストケースにおいては「全参加者中の最小絶対スコア」の計算から除外される。
システムテストは
<font color="red">
<strong>

<span>
CE
</span>
以外の結果を得た一番最後の提出
</strong>
</font>
に対してのみ行われるため、最終的に提出する解答を間違えないよう注意せよ。
</p>

#### **テストケース数**

<ul>

<li>
暫定テスト: 50個
</li>

<li>
システムテスト: 3000個、コンテスト終了後に <a href="https://img.atcoder.jp/ahc045/seeds.txt">seeds.txt</a>(sha256=e4cb8e03f20f6a97dd082c75ad60cc31447bd24b5b3ebe5e64af4ac28712b618) を公開
</li>

</ul>

#### **相対評価システムについて**

<p>
暫定テスト、システムテストともに、
<span>
CE
</span>
以外の結果を得た一番最後の提出のみが順位表に反映される。
相対評価スコアの計算に用いられる各テストケース毎の全参加者中の最小絶対スコアの算出においても、順位表に反映されている最終提出のみが用いられる。
</p>

<p>
順位表に表示されているスコアは相対評価スコアであり、新規提出があるたびに、相対評価スコアが再計算される。
一方、提出一覧から確認出来る各提出のスコアは各テストケース毎の絶対スコアをそのまま足し合わせたものであり、相対評価スコアは表示されない。
最新以外の提出の、現在の順位表における相対評価スコアを知るためには、再提出が必要である。
不正な出力や制限時間超過をした場合、提出一覧から確認出来るスコアは0となるが、順位表には正解したテストケースに対する相対スコアの和が表示されている。
</p>

#### **実行時間について**

<p>
実行時間には多少のブレが生じます。
また、システムテストでは同時に大量の実行を行うため、暫定テストに比べて数%程度実行時間が伸びる現象が確認されています。
そのため、実行時間制限ギリギリの提出がシステムテストで
<span>
TLE
</span>
となる可能性があります。
プログラム内で時間を計測して処理を打ち切るか、実行時間に余裕を持たせるようお願いします。
</p>

</section>

</div>

<div>

<section>

### **入出力**

<p>
まず初めに、都市の個数 $N$、回答における都市のグループの個数 $M$、最大クエリ回数 $Q$、クエリを行う都市の集合のサイズの上限 $L$、都市の座標が含まれる長方形の幅や高さとして有り得る最大値 $W$、各グループに割り当てる都市の個数を表す配列 $G$、各都市が存在する可能性のある座標の長方形範囲 $lx_i, rx_i, ly_i, ry_i$が、以下の形式で標準入力から与えられる。
</p>

<div>

$N$$M$$Q$$L$$W$$G_0$$G_1$$\cdots$$G_{M-1}$$lx_0$$rx_0$$ly_0$$ry_0$$\vdots$$lx_{N-1}$$rx_{N-1}$$ly_{N-1}$$ry_{N-1}$
</div>

<p>
各値はそれぞれ以下の制約を満たす。
</p>

<ul>

<li>
$N = 800$
</li>

<li>
$1 \leq M \leq 400$
</li>

<li>
$Q = 400$
</li>

<li>
$3 \leq L \leq 15$
</li>

<li>
$500 \leq W \leq 2500$
</li>

<li>
$1 \leq G_i \leq N$
</li>

<li>
$\sum_{i=0}^{M-1} G_i = N$
</li>

<li>
$0 \leq lx_i \leq rx_i \leq 10000$
</li>

<li>
$0 \leq rx_i - lx_i \leq W$
</li>

<li>
$0 \leq ly_i \leq ry_i \leq 10000$
</li>

<li>
$0 \leq ry_i - ly_i \leq W$
</li>

<li>
入力は全て整数である。
</li>

</ul>

<p>
上記の情報を読み込んだ後、以下のクエリを最大 $Q$回まで繰り返す。
</p>

<p>
各クエリでは、都市の集合 $C \subset \{0,1,\cdots,N-1\}$を選ぶ。ただし、その大きさ $l = |C|$は入力で指定される上限サイズ $L$に対して $2 \le l \le L$を満たす必要がある。
これらの値を以下の形式で一行で標準出力に出力せよ。
</p>

<div>

$\mathrm{?}$$l$$C_0$$C_1$$\cdots$$C_{l-1}$
</div>

<p>

<font color="red">
<strong>
出力の後には改行をし、更に標準出力を flush しなければならない。
</strong>
</font>
そうしない場合、
<span>
TLE
</span>
となる可能性がある。
</p>

<p>
出力後に、都市集合 $C$上での最小全域木を構成するための $l-1$本の道路それぞれが接続する都市の組 $a_i, b_i \in C$が、以下の形式で標準入力から与えられる。
</p>

<div>

$a_0$$b_0$$\vdots$$a_{l-2}$$b_{l-2}$
</div>

<p>
最大 $Q$回までのクエリ処理が完了後、まず初めに記号 $\mathrm{!}$のみを一行で標準出力に出力せよ。
</p>

<div>

$\mathrm{!}$
</div>

<p>
その後、各グループに対する回答を以下の形式で $M$グループ分繰り返し出力せよ。
グループ $k$に対する回答では、そのグループに割り当てる都市の集合 $C \subset \{0,1,\cdots,N-1\}$と、その都市間を結ぶ道路の組 $a_i, b_i \in C$を以下の形式で出力せよ。
</p>

<div>

$C_0$$C_1$$\cdots$$C_{G_k-1}$$a_0$$b_0$$\vdots$$a_{G_k-2}$$b_{G_k-2}$
</div>

<p>
この時、出力は以下の制約を満たす必要がある。
</p>

<ul>

<li>
各都市は必ず1つのグループに割り当てられる。どのグループにも割り当てられない都市や、複数のグループに割り当てられる都市は存在しない。
</li>

<li>
各グループ内の任意の2都市間は道路によって相互に到達可能、すなわちグラフとして連結である。
</li>

</ul>

#### **例**

<table>

<thead>

<tr>

<th>
$q$
</th>

<th>
Output
</th>

<th>
Input
</th>

</tr>

</thead>

<tbody>

<tr>

<td>
事前情報
</td>

<td>

</td>

<td>

<div>

5 2 3 3 500
3 2
1375 1648 351 624
1773 1900 3660 3787
2922 3231 558 867
5358 5640 8585 8867
3218 3684 3330 3796

</div>

</td>

</tr>

<tr>

<td>
0
</td>

<td>

<div>

? 3 4 1 2
</div>

</td>

<td>

<div>

1 4
2 4

</div>

</td>

</tr>

<tr>

<td>
1
</td>

<td>

<div>

? 3 1 3 4
</div>

</td>

<td>

<div>

1 4
3 4

</div>

</td>

</tr>

<tr>

<td>
回答
</td>

<td>

<div>

!
3 4 1
3 4
1 4
2 0
0 2

</div>

</td>

</tr>

</tbody>

</table>

<p>
<a href="https://img.atcoder.jp/ahc045/jOO09LxU.html?lang=ja&seed=0&output=sample">例を見る</a>
</p>

</section>

</div>

<div>

<section>

### **入力生成方法**

<p>
$L$以上 $U$以下の整数値を一様ランダムに生成する関数を $\mathrm{rand\_int}(L,U)$、
$L$以上 $U$未満の実数値を一様ランダムに生成する関数を $\mathrm{rand\_double}(L,U)$で表す。
</p>

#### **$M, L, W$の生成**

<ul>

<li>
$M = \left\lfloor (\mathrm{rand\_double}(1.0, 20.0))^2 \right\rfloor$
</li>

<li>
$L = \mathrm{rand\_int}(3, 15)$
</li>

<li>
$W = \mathrm{rand\_int}(500, 2500)$
</li>

</ul>

#### **$G$の生成**

<ul>

<li>
$1$以上 $N-1$以下の整数値を、重複しないようにして一様ランダムに $M-1$個生成し、昇順に並べたものを $A_1, A_2, \cdots, A_{M-1}$とする。
</li>

<li>
$A_0 = 0, A_M = N$として、$G_i = A_{i+1} - A_i$とする。
</li>

</ul>

#### **$x_i, y_i, lx_i, rx_i, ly_i, ry_i$の生成**

<ul>

<li>
$x_i = \mathrm{rand\_int}(0, 10000)$
</li>

<li>
$y_i = \mathrm{rand\_int}(0, 10000)$
</li>

<li>
$w_i = \mathrm{rand\_int}(0, W)$
</li>

<li>
$dx_i = \mathrm{rand\_int}(0, w_i)$
</li>

<li>
$rx_i = x_i + dx_i$
</li>

<li>
$lx_i = rx_i - w_i$
</li>

<li>
$dy_i = \mathrm{rand\_int}(0, w_i)$
</li>

<li>
$ry_i = y_i + dy_i$
</li>

<li>
$ly_i = ry_i - w_i$
</li>

<li>
$lx_i, rx_i, ly_i, ry_i$が $0$未満の場合は $0$に、 $10000$を超える場合は $10000$に置き換える。
</li>

</ul>

</section>

</div>

<div>

<section>

### **ツール(入力ジェネレータ・ビジュアライザ)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc045/jOO09LxU.html?lang=ja">Web版</a>: ローカル版より高性能でアニメーション表示が可能です。
</li>

<li>
<a href="https://img.atcoder.jp/ahc045/jOO09LxU_v2.zip">ローカル版</a>: 使用するには<a href="https://www.rust-lang.org/ja">Rust言語</a>のコンパイル環境をご用意下さい。
<ul>

<li>
<a href="https://img.atcoder.jp/ahc045/jOO09LxU_windows_v2.zip">Windows用のコンパイル済みバイナリ</a>: Rust言語の環境構築が面倒な方は代わりにこちらをご利用下さい。
</li>

</ul>

</li>

</ul>

<p>

<font color="red">
<b>
コンテスト期間中に、ビジュアライズ結果の共有や、解法・考察に関する言及は禁止されています。ご注意下さい。
</b>
</font>

</p>

#### **ツールで用いられる入出力ファイルの仕様**

<p>
ローカルテスタに与える入力ファイルは解答プログラムに与えられる事前情報の末尾に以下の形式の情報が追加されている。
</p>

<div>

$x_0$$y_0$$\vdots$$x_{N-1}$$y_{N-1}$
</div>

<p>
$x_i,y_i$は都市 $i$の真の座標であり、解答プログラムには与えられない。
</p>

</section>

</div>

<div>

<section>

### **サンプルプログラム**

<details>

<summary>
Pythonによるサンプル実装
</summary>

```
def query(c):
    print("?", len(c), *c, flush=True)
    return [tuple(map(int, input().split())) for _ in range(len(c) - 1)]


def answer(groups, edges):
    print("!")
    for i in range(len(groups)):
        print(*groups[i])
        for e in edges[i]:
            print(*e)


# read input
N, M, Q, L, W = map(int, input().split())
G = list(map(int, input().split()))
lx, rx, ly, ry = [], [], [], []
for _ in range(N):
    a, b, c, d = map(int, input().split())
    lx.append(a)
    rx.append(b)
    ly.append(c)
    ry.append(d)

# use center of rectangle
x = [(l + r) // 2 for l, r in zip(lx, rx)]
y = [(l + r) // 2 for l, r in zip(ly, ry)]

# split cities into groups
cities = list(range(N))
cities.sort(key=lambda i: (x[i], y[i]))
groups = []
start_idx = 0
for g in G:
    groups.append(cities[start_idx : start_idx + g])
    start_idx += g

# get edges from queries
edges = []
for k in range(M):
    edges.append([])
    for i in range(0, G[k] - 1, 2):
        if i < G[k] - 2:
            ret = query(groups[k][i : i + 3])
            edges[k].extend(ret)
        else:
            edges[k].append(groups[k][i : i + 2])

# output answer
answer(groups, edges)

```

</details>

<p>
以下の処理を実装しています。
</p>

<ol>

<li>
都市を与えられた長方形範囲の中心座標 $(\frac{lx_i + rx_i}{2}, \frac{ly_i + ry_i}{2})$でソートし、その順番でグループに分割する。
</li>

<li>
各グループについて、3都市クエリを2都市ずつスライドしながら行い、クエリの応答として得られた辺をそのまま回答に追加する。
</li>

<li>
各グループについて最後の都市がクエリできなかった場合は、グループ内の直前の都市との辺を回答に追加する。
</li>

</ol>

</section>

</div>

</span>

</span>

</div>
