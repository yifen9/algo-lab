
<div>

<span>

<span>

<p>
Score : $675$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Takahashi and Aoki play a card game. The game proceeds according to the following rules.  
</p>

<ul>

<li>
Takahashi presents decks $A_1, A_2, \dots, A_N$. Here $N \geq 3$.
</li>

<li>
Aoki presents decks $B_1, B_2, B_3$.
</li>

<li>
Takahashi chooses one deck from Aoki's decks and bans it. Aoki also chooses one deck from Takahashi's decks and bans it. These two ban operations are performed 
<strong>
simultaneously
</strong>
. (That is, neither player can act based on the other's choice.)
</li>

<li>
Then, Takahashi and Aoki each 
<strong>
simultaneously
</strong>
declare which deck from their own presented decks they will use. However, the banned deck cannot be declared.
</li>

<li>
Then, the two players battle exactly once using their declared decks. As a result, one of them wins.
</li>

</ul>

<p>
You are given integers $X_{i,j}$$(1 \leq i \leq N, 1 \leq j \leq 3)$. Let $p_{i,j} = \dfrac{X_{i,j}}{10^6}$. $p_{i,j}$is Takahashi's win rate when Takahashi uses deck $A_i$and Aoki uses deck $B_j$. Both Takahashi and Aoki know the values of $p_{i,j}$in advance.

Find Takahashi's win rate when both players act to maximize their own win rate.
</p>

<p>
$T$test cases are given; solve each of them.
</p>

<details>

<summary>
What is Takahashi's win rate when both players act to maximize their own win rate?
</summary>
At each stage, each player assigns probabilities summing to $1$to the available choices based on the information revealed up to that point, and randomly selects one choice according to those probabilities.

Each player chooses a strategy that maximizes "the minimum possible win rate," that is, "the win rate when the opponent chooses a strategy that minimizes the player's win rate." If there are multiple strategies satisfying this condition, any of them may be chosen.

When both players act according to this policy, Takahashi's win rate is uniquely determined regardless of the specific strategy chosen. Find this value.


</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq 500$
</li>

<li>
$3 \leq N \leq 5 \times 10^4$
</li>

<li>
$0 \leq X_{i,j} \leq 10^6$
</li>

<li>
The sum of $N$over all test cases is at most $5 \times 10^4$.
</li>

<li>
All input values are integers.
</li>

</ul>

</section>

</div>

---

<div>

<div>

<section>

### **Input**

<p>
The input is given from Standard Input in the following format, where $\mathrm{case}_i$denotes the $i$-th test case.
</p>

<div>

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
For each test case, the input is given in the following format.
</p>

<div>

$N$$X_{1,1}$$X_{1,2}$$X_{1,3}$$X_{2,1}$$X_{2,2}$$X_{2,3}$$\vdots$$X_{N,1}$$X_{N,2}$$X_{N,3}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line should contain the answer to the $i$-th test case.

For each test case, output Takahashi's win rate when both players act to maximize their own win rate. The output is considered correct if the absolute or relative error from the true value is at most $10^{-6}$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

1
3
600000 500000 100000
400000 700000 300000
800000 200000 900000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

0.5272727272727272

</div>

<p>
Takahashi's win rate when both players act to maximize their own win rate is $0.5272727 \cdots$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
6
402522 269943 705465
529104 292257 262398
598965 708517 393767
10680 760196 459175
163269 555933 100458
252724 762224 143581
4
720086 398924 165990
446155 678065 592893
674921 176800 484411
222632 81476 633357
5
212176 543920 484352
23874 760886 95861
291354 504948 790821
523486 327166 289413
621589 178581 628701

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0.5136657634439492
0.5120053615937050
0.5396248345565982

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

6
3
600000 300000 100000
0 400000 600000
700000 400000 100000
3
700000 700000 200000
0 0 900000
500000 600000 900000
5
1000000 658525 1000000
867635 1000000 259903
727305 342912 1000000
995128 432824 1000000
69492 105991 1000000
6
900000 700000 300000
600000 300000 500000
900000 100000 900000
900000 1000000 0
800000 200000 900000
700000 800000 900000
7
300000 900000 800000
600000 1000000 700000
700000 200000 1000000
1000000 200000 200000
200000 400000 1000000
500000 800000 900000
900000 500000 800000
5
500000 500000 41274
270488 520436 605863
247128 522516 149943
502751 491747 516407
503752 488744 31814

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

0.3520000000000000
0.5571428571428572
0.9951279999999999
0.8478260869565216
0.8336956521739129
0.4988562153245037

</div>

</section>

</div>

</span>

</span>

</div>
