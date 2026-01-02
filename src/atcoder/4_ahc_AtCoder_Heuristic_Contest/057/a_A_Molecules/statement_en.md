
<div>

<span>

<span>

<div>

<section>

### **Story**

<p>
AtCoder Laboratory is engaged in the development of new molecules.
Takahashi, a genius chemist, can freely bond atoms that move around at any timing he chooses to form molecules.
However, bonding atoms consumes energy depending on the distance between them, so he wants to create the required number of molecules using as little energy as possible.
</p>

</section>

</div>

<div>

<section>

### **Problem Statement**

<p>
Consider a two-dimensional plane defined by $0 \leq x < L = 10^5$and $0 \leq y < L = 10^5$. This plane has a <a href="https://en.wikipedia.org/wiki/Torus">toroidal</a>structure, meaning the left and right edges ($x = 0$and $x = L$), as well as the top and bottom edges ($y = 0$and $y = L$), are connected. Any coordinates outside this range are normalized to fall within $0 \leq x, y < L$by taking the remainder when divided by $L$for both $x$and $y$. For example, the position reached by moving $(-20000, 30000)$from $(10000, 90000)$is $(90000, 20000)$.
</p>

<p>
There are $N$points on this plane. At time $t = 0$, the initial position $(x_i, y_i)$($0 \leq x_i, y_i < L$) and initial velocity $(vx_i, vy_i)$($-100 \leq vx_i, vy_i \leq 100$) of the $i$-th point ($0 \leq i < N$) are given as input. In the initial state, each point forms an independent connected component.
</p>

<p>
At each time $t = 0, 1, \ldots, T - 1$, the following two phases are processed in order: 
<strong>
1. Bonding Phase
</strong>
and 
<strong>
2. Movement Phase
</strong>
.
</p>

<p>

<strong>
1. Bonding Phase
</strong>

</p>

<p>
At time $t$, it is possible to 
<strong>
bond
</strong>
two points that belong to different connected components. Multiple bonds may be performed in the same time step.
</p>

<p>
Let $(x_i, y_i)$be the position of point $i$at time $t$, and $(x_j, y_j)$be the position of point $j$at time $t$. The 
<strong>
bonding cost
</strong>
$D$for bonding point $i$and point $j$is calculated using the following distance formula:
</p>

<p>
\[
  D = \mathrm{round}\left(
    \sqrt{
      \bigl(\min(L - \Delta x,\ \Delta x)\bigr)^2
      +
      \bigl(\min(L - \Delta y,\ \Delta y)\bigr)^2
    }
  \right)
\]
</p>

<p>
\[
  \Delta x = |x_i - x_j|,\quad \Delta y = |y_i - y_j|
\]
</p>

<p>
When two points are bonded, the velocity of the resulting connected component is updated according to the law of conservation of momentum. Suppose that before the bond, point $i$belongs to connected component $A$moving at velocity $(vx_A, vy_A)$, and point $j$belongs to connected component $B$moving at velocity $(vx_B, vy_B)$. Then, for all points belonging to connected components $A$and $B$, the velocity $(vx_{\text{new}}, vy_{\text{new}})$after bonding is updated as follows:
</p>

<p>
\[
(vx_{\text{new}}, vy_{\text{new}}) =
\left(
\frac{|A| \times vx_A + |B| \times vx_B}{|A| + |B|},
\frac{|A| \times vy_A + |B| \times vy_B}{|A| + |B|}
\right)
\]
</p>

<p>
Here, $|A|$and $|B|$denote the number of points in connected components $A$and $B$, respectively. After bonding, all points in the resulting connected component will move with 
<strong>
the same velocity
</strong>
. The positions of the points do not change due to bonding. Additionally, the order in which bonds are performed within the same time step does not affect the resulting positions, bonding costs, or velocities of the connected components.
</p>

<p>
Coordinates and velocities may become fractional, but all computations are performed using double-precision floating-point arithmetic.
</p>

<p>

<strong>
2. Movement Phase
</strong>

</p>

<p>
The positions of all points in each connected component are updated simultaneously. Let $(x_i, y_i)$be the position of point $i$at time $t$, and let $(vx_i, vy_i)$be the velocity of the connected component to which point $i$belongs. Then, the position $(x_i', y_i')$of point $i$at time $t + 1$is updated as follows:
</p>

<p>
\[
(x_i', y_i') = ((x_i + vx_i) \bmod L,  (y_i + vy_i) \bmod L)
\]
</p>

<p>
Plan the bonds so that at time $T$, the number of connected components is 
<strong>
exactly $M$
</strong>
, and the size of each connected component is 
<strong>
exactly $K$
</strong>
, while minimizing the 
<strong>
total bonding cost $D$
</strong>
.
</p>

#### **Example of Bonding and Movement**

<blockquote>

<p>

<img src="https://img.atcoder.jp/ahc057/BJTm8xSg.gif">

</img>

</p>

<p>
The figure above illustrates an example of bonding three points into a single connected component.
First, the two points at the lower left and lower right are bonded, and their direction of movement changes upward.
Next, they are bonded with the point moving to the right at the top, and the direction of movement changes to upward-right.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Scoring**

<p>
Let the total bonding cost of all bonds be $D_{\text{sum}}$. The score for a single test case is calculated as follows. A higher score is better.
</p>

<p>
\[
\mathrm{Score} = \mathrm{round}\!\left(10^{6} \times \log_{2}\!\left( \frac{L \times (N - M)}{D_{\text{sum}} + 1} \right)\right)
\]
</p>

<p>
The result will be 
<span>
WA
</span>
in the following cases:
</p>

<ul>

<li>
If the output is invalid  
</li>

<li>
If at time $T$, the number of connected components is not 
<strong>
exactly $M$
</strong>
, or the size of each connected component is not 
<strong>
exactly $K$
</strong>

</li>

<li>
If a bond is specified between two points that already belong to the same connected component
</li>

</ul>

<p>
There are $150$test cases, and the score of a submission is the total score for each test case.
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

$N$$T$$M$$K$$L$$x_0$$y_0$$vx_0$$vy_0$$x_1$$y_1$$vx_1$$vy_1$$\vdots$$x_{N-1}$$y_{N-1}$$vx_{N-1}$$vy_{N-1}$
</div>

<ul>

<li>
The total number of points is $N = 300$.  
</li>

<li>
The total number of steps is $T = 1000$.  
</li>

<li>
The target number of connected components is $M = 10$.  
</li>

<li>
The target size of each connected component is $K = 30$.  
</li>

<li>
The side length of the space is $L = 10^5$.  
</li>

<li>
$(x_i, y_i)$represents the initial position of point $i$, where $0 \leq x_i, y_i < L$and values are integers.  
</li>

<li>
$(vx_i, vy_i)$represents the initial velocity of point $i$, where $-100 \leq vx_i, vy_i \leq 100$and values are integers.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output exactly $N - M$lines to Standard Output. Each line consists of the following three integers, representing that point $i$and point $j$are bonded at time $t$.
The order of the output is arbitrary, but the processing is performed in ascending order of time $t$.
</p>

<div>

$t$$i$$j$
</div>

<p>
The output must satisfy the following conditions:
</p>

<ul>

<li>
$0 \leq t < T$
</li>

<li>
$0 \leq i, j < N$, and $i \neq j$
</li>

</ul>

<p>
<a href="https://img.atcoder.jp/ahc057/BJTm8xSg.html?lang=en&seed=0&output=sample">Show example</a>
</p>

</section>

</div>

<div>

<section>

### **Input Generation**

<p>
$\mathrm{rand}(L,U)$: Randomly generates an integer between $L$and $U$, inclusive, with uniform probability.
</p>

<p>

<strong>
Generating Initial Positions
</strong>

</p>

<p>
For each point $i$, independently generate $x_i = \mathrm{rand}(0, L - 1)$and $y_i = \mathrm{rand}(0, L - 1)$.
</p>

<p>

<strong>
Generating Initial Velocities
</strong>

</p>

<p>
For each point $i$, independently generate $vx_i = \mathrm{rand}(-100, 100)$and $vy_i = \mathrm{rand}(-100, 100)$.
</p>

</section>

</div>

<div>

<section>

### **Tools (Input generator and visualizer)**

<ul>

<li>
<a href="https://img.atcoder.jp/ahc057/BJTm8xSg.html?lang=en">Web version</a>: This is more powerful than the local version providing animations.
</li>

<li>
<a href="https://img.atcoder.jp/ahc057/BJTm8xSg.zip">Local version</a>: You need a compilation environment of <a href="https://www.rust-lang.org/">Rust language</a>.
<ul>

<li>
<a href="https://img.atcoder.jp/ahc057/BJTm8xSg_windows.zip">Pre-compiled binary for Windows</a>: If you are not familiar with the Rust language environment, please use this instead.
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

300 1000 10 30 100000
2436 18582 80 -53
11172 25071 -47 -71
56643 73929 46 -89
32441 4016 1 62
81600 85102 -62 83
46831 96411 -13 -88
85958 91609 -31 -51
47788 53885 -98 87
80068 86751 -32 23
73792 28207 -18 55
82502 35092 87 41
42677 29047 14 -3
20208 44400 80 4
81416 25817 -66 85
66324 4956 19 73
79260 68753 -99 97
60669 49104 -1 -68
11487 8219 96 82
10449 35974 97 -83
36934 26216 -57 12
31832 45833 7 -75
84066 42632 -42 -93
48899 22095 -20 4
499 17907 19 -59
58093 41209 -45 61
68394 86597 7 16
94459 57728 47 38
3355 90413 64 -42
86511 77344 -16 -73
61617 76222 69 84
36013 78203 -62 -7
66418 15805 -100 -12
62210 76124 -63 78
69486 84752 96 -4
62365 49587 -35 3
7036 85915 -25 -91
85117 52902 -6 -95
30509 85473 -47 -80
85969 88350 -86 42
75340 91696 -48 -99
4902 94732 -49 49
44596 90771 -37 48
44827 68181 80 -98
96068 81537 -61 -35
92964 85388 -61 29
30384 93176 19 23
16047 68444 -56 -61
72556 4749 11 -17
41093 18686 -9 -10
73474 10624 89 39
38347 89510 -90 57
63568 16873 51 75
87374 7602 70 69
50016 50344 46 -6
72135 90944 -60 20
79124 34278 -14 85
57903 91370 -82 -86
65699 24840 -90 71
61416 42823 -4 -27
5881 13273 -75 35
90608 55227 44 26
4228 84079 -51 23
63053 6894 -83 20
54427 32840 -98 0
35069 866 60 84
56338 3161 -1 -67
87839 68526 -17 87
51927 22524 62 -88
18360 76668 -49 -19
41330 38632 -43 85
8423 85430 27 -72
31151 30949 -35 -68
35425 98667 -34 -40
64216 29899 -17 40
6406 50469 75 81
55655 37416 -9 35
1516 30683 82 35
91220 8358 -5 43
17134 28374 68 41
33754 62967 -80 79
49343 85380 -81 91
42151 35142 65 -92
66104 39335 71 9
14111 50565 -100 51
89806 40162 32 -37
64785 72129 20 31
32720 22985 29 53
72911 9918 46 -92
49311 20410 -27 -28
67923 29578 26 -75
35876 65903 32 -37
56965 81112 92 -12
69550 59002 36 35
63834 92908 -88 -19
75066 80665 47 -88
53110 24554 -90 54
59597 4126 20 -11
63411 98916 -27 -16
78646 71220 -6 18
53418 70370 -79 -22
91062 85140 -67 -83
86010 32629 2 45
75168 84052 24 48
85615 38954 18 19
13168 93699 30 -42
77158 13596 -79 -73
99380 68100 8 70
42694 41699 -32 96
57174 23983 44 -64
88856 48119 71 -2
57945 26398 -96 16
34332 3616 61 -76
20394 35156 22 -58
68780 41704 50 -73
5379 44220 55 21
90510 66235 28 -92
69428 77407 51 5
10696 78430 -45 -40
24277 96652 39 90
81795 3062 99 -31
80424 39645 -26 -51
62404 61793 1 42
18353 74523 -48 46
28270 6207 47 56
15533 8441 36 -4
83297 59770 17 -87
85877 26141 49 5
77103 62145 -32 -29
90325 58414 94 -90
26573 75460 31 -73
4974 24976 97 -93
28525 86194 20 74
83856 264 18 21
74580 51154 15 48
50869 29907 -6 78
948 12466 -82 -46
7689 60224 -42 -21
44985 60022 11 10
45567 21013 -71 40
41314 93936 92 -63
95718 29800 -8 -53
60008 67095 78 29
55013 36137 87 -66
503 3718 36 64
43856 81799 -81 19
91386 79466 -62 15
8026 98878 97 -6
96002 46215 -50 -42
54713 50659 9 -42
89363 21620 -56 19
49962 67038 55 -15
943 41697 7 53
40087 42225 16 -47
57254 77442 98 -82
36337 29590 74 91
26938 3423 54 51
39779 32823 -77 -84
32847 17135 100 -5
79055 40811 92 -15
21868 98831 -91 -38
10449 6999 -82 35
49418 87285 -42 37
97197 74822 -17 10
47348 63144 -90 68
64915 22253 74 90
42086 35915 -53 23
18935 26845 77 -20
2238 2244 41 32
72456 93027 -41 0
28617 20552 -62 -80
94701 39336 12 -49
62123 63790 58 -46
99993 60564 -69 2
3426 80446 52 -73
30321 10476 -70 -21
23253 950 28 -100
44526 84781 -56 57
51852 64272 -72 -78
84201 88938 -26 63
86769 34382 22 -32
22189 86673 62 9
58373 8944 -9 46
53079 90631 -48 29
23413 91072 45 66
88867 741 -23 16
1384 41908 95 76
35135 90166 -26 -95
74179 9930 -48 -51
50994 17019 27 -91
5797 76408 -10 4
96854 40045 64 34
92623 24149 -16 -69
83586 30280 -10 -26
61804 51797 31 -94
46036 49587 -32 -55
37530 39036 -59 69
8874 85829 -22 90
7485 2200 50 30
67407 98154 94 -30
70157 77324 48 34
81873 76890 39 58
52818 91109 22 -17
54658 95263 37 -59
9119 34477 25 -93
7129 74354 -18 25
60889 27731 -21 48
24786 2060 45 -46
38075 19541 38 -66
98098 20038 -52 10
35468 98666 34 -11
41880 19402 82 64
87283 93233 83 27
82643 48079 -82 85
36106 27889 49 -31
70284 84426 80 -34
48079 65974 -33 31
38620 22820 82 -33
12105 891 -35 3
39572 8070 -6 -100
88044 22119 28 -49
15634 33732 -100 -15
28278 92300 19 67
31771 58716 -81 49
3779 44317 -96 52
42251 33963 67 -2
2716 85833 -9 -22
94473 45427 -11 27
57546 98190 -38 33
93488 69325 88 -86
16834 84421 68 -24
16776 36469 87 -8
30469 55819 9 91
66676 94952 -51 100
74225 42292 -64 27
95178 98882 16 72
41586 53226 72 -25
54425 28395 40 86
63295 44650 35 -8
8918 89927 -84 -58
43617 54136 84 29
19114 90718 -88 -81
11772 48502 58 50
16769 18178 -52 10
30990 46183 53 87
77588 15246 75 73
22840 26416 74 -49
83985 39929 53 -81
47630 92407 -85 97
47626 93543 79 -6
66366 61019 98 -12
78834 90305 15 27
68799 66940 -16 45
84458 86826 83 1
96854 48119 -12 -81
28842 45332 -3 -85
99589 87666 68 28
10768 6116 4 13
77087 97715 93 60
19218 20594 73 -99
43766 43938 -29 69
36059 6277 30 -42
61262 71995 -14 54
53727 87806 -50 95
68498 24075 68 66
65701 58821 -43 -33
26807 3006 -99 78
96611 40954 -32 -61
74332 68414 61 -41
93886 14955 42 77
65492 15419 57 -3
92243 49163 -85 44
51731 74047 62 -54
98816 47865 4 -27
97740 87273 91 -72
67507 30632 34 -35
4098 14515 -92 93
99437 70562 11 -78
84641 87942 -56 -81
58040 49980 -94 8
66894 70330 57 89
49916 43921 -1 31
46384 60472 -58 17
76985 7656 -92 54
76463 7654 -42 74
67955 20110 74 -3
86395 65532 45 -52
80133 44506 -16 -19
3979 57651 65 -65
67184 14011 -99 48
26965 3647 -19 -29
97237 34716 16 -20
44259 87431 62 21
2929 5456 69 -8
82897 12715 12 5
46414 16319 54 43
20952 55289 -73 21
32306 80650 -36 -37
32354 54519 81 -4
22913 77540 -61 -66
21963 14649 67 -28

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

510 192 66
226 174 276
569 16 98
958 56 36
744 30 149
936 81 236
289 260 269
289 276 222
69 146 210
81 107 230
842 25 199
746 82 230
103 68 143
986 39 60
159 58 241
908 247 80
512 274 216
167 154 138
881 220 241
392 59 54
841 235 190
625 206 246
267 69 138
290 177 163
708 116 55
424 52 66
156 291 14
476 130 213
122 189 155
457 226 136
866 34 163
767 29 292
496 74 22
772 172 237
28 139 1
591 88 20
219 140 47
626 191 68
180 209 150
626 279 265
4 73 20
319 156 136
775 97 231
358 141 154
488 85 254
39 164 180
30 83 21
150 197 163
162 217 222
780 152 71
67 282 88
642 133 254
617 248 95
134 86 128
291 4 116
44 178 206
554 79 66
319 117 92
202 254 253
56 3 153
801 168 231
933 122 65
990 180 54
485 26 294
703 251 123
438 44 77
821 222 262
188 232 160
661 112 258
697 277 83
596 228 244
682 91 221
976 281 20
772 160 0
732 236 143
173 57 282
7 144 16
343 183 244
691 294 194
61 241 163
463 280 5
157 27 247
555 105 65
105 55 119
206 41 125
770 124 199
318 297 181
357 250 269
220 110 197
373 76 151
449 9 164
507 287 92
436 171 35
552 285 102
862 63 36
553 244 163
576 292 194
308 106 107
546 138 229
15 163 87
297 128 173
959 23 39
284 123 154
720 126 68
687 5 117
757 272 134
966 270 259
926 216 149
407 120 199
907 198 262
764 157 54
744 227 181
423 121 73
650 0 12
44 230 229
926 245 59
11 239 228
317 37 207
932 268 118
55 252 138
33 99 16
504 62 36
303 296 206
623 28 55
726 293 80
284 72 19
924 153 246
928 267 131
752 181 54
833 150 214
541 115 194
418 237 236
418 113 153
673 78 73
254 185 233
81 71 267
403 46 12
317 67 184
130 103 28
827 93 46
327 210 276
731 199 119
647 223 116
525 255 131
903 19 44
207 208 78
406 40 245
102 205 271
544 188 230
202 65 261
145 213 131
509 14 131
374 215 252
751 145 77
658 95 287
711 243 12
180 196 79
840 108 79
74 109 296
869 94 125
73 179 20
328 96 161
444 155 18
413 170 73
930 38 271
197 169 236
927 290 132
869 45 68
656 90 197
739 75 216
173 7 214
671 283 83
143 53 117
687 125 93
667 89 124
246 286 56
168 36 93
29 187 137
256 263 187
196 231 137
478 15 63
848 167 44
482 211 199
864 92 225
795 289 128
293 278 285
422 161 163
571 257 160
359 242 241
172 299 1
377 35 157
204 47 256
979 80 28
950 288 28
598 114 20
636 166 73
175 275 47
306 84 183
850 162 220
816 238 182
947 225 194
420 259 262
827 219 213
665 66 137
785 240 241
105 151 150
972 118 246
857 104 78
59 8 272
903 295 36
251 265 150
202 284 256
223 201 114
3 158 229
290 135 0
157 48 84
809 102 4
411 224 156
461 193 28
342 262 269
882 149 50
530 49 269
458 271 92
125 253 137
97 195 260
536 261 153
153 218 163
714 176 20
251 159 225
729 17 182
121 132 51
882 18 119
201 6 229
232 143 246
715 64 120
781 173 218
118 186 241
443 207 92
163 142 146
236 1 151
176 42 53
883 264 113
387 148 20
871 33 14
751 32 49
569 22 236
938 249 93
11 98 213
707 10 105
285 134 146
27 50 114
56 204 247
117 61 296
388 258 20
471 147 112
129 221 210
403 234 73
863 131 273
490 54 137
337 175 192
748 256 222
283 190 6
99 11 141
528 212 128
748 203 197
330 233 184
189 2 139
66 31 159
162 77 225
581 21 229
89 51 0
44 165 134
782 101 277
275 100 73
189 298 258
921 24 191
518 70 86
149 43 265
913 13 82
471 127 121
199 184 229
132 136 12
51 182 36
240 214 273
314 200 159
923 202 138
997 266 222
28 60 28
267 111 273
460 129 140

</div>

</section>

</div>

</span>

</span>

</div>
