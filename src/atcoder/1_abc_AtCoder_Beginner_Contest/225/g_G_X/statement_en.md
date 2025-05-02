
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
We have a grid with $H$horizontal rows and $W$vertical columns. Each square contains an integer. The square $(i, j)$at the $i$-th row from the top and $j$-th column from the left contains the integer $A_{i,j}$.
</p>

<p>
Takahashi will choose zero or more from the $H \times W$squares and draw an X on each of them. An X is composed of a segment connecting the top-left and bottom-right corners, and a segment connecting the top-right and bottom-left corners.
</p>

<p>
Let us define Takahashi's score as $($the sum of integers contained in the squares on which X is drawn$) - C \times ($the minimum number of segments needed to draw the X's$)$.
</p>

<p>
Here, Takahashi can draw X's on diagonally adjacent squares at once.
</p>

<p>
For example, he can draw X's on the squares $(1, 1)$and $(2, 2)$with three segments:
</p>

<ul>

<li>
a segment connecting the top-left corner of $(1, 1)$and the bottom-right corner of $(2, 2)$,
</li>

<li>
a segment connecting the top-right corner of $(1, 1)$and the bottom-left corner of $(1, 1)$,
</li>

<li>
a segment connecting the top-right corner of $(2, 2)$and the bottom-left corner of $(2, 2)$.
</li>

</ul>

<p>
Find Takahashi's maximum possible score. 
<strong>
Note that nothing should be drawn on unchosen squares.
</strong>

</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq H,W \leq 100$
</li>

<li>
$1 \leq C \leq 10^9$
</li>

<li>
$1 \leq A_{i,j} \leq 10^9$
</li>

<li>
All values in input are integers.
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
Input is given from Standard Input in the following format:
</p>

<div>

$H$$W$$C$$A_{1,1}$$A_{1,2}$$\ldots$$A_{1,W}$$A_{2,1}$$A_{2,2}$$\ldots$$A_{2,W}$$\hspace{1.5cm}\vdots$$A_{H,1}$$A_{H,2}$$\ldots$$A_{H,W}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print Takahashi's maximum possible score.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2 2 2
2 10
8 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

12

</div>

<p>
If he chooses the squares $(1,2)$and $(2,1)$, he can draw X's on them with three segments:
</p>

<ul>

<li>
a segment connecting the top-left corner of $(1, 2)$and the bottom-right corner of $(1, 2)$,
</li>

<li>
a segment connecting the top-left corner of $(2, 1)$and the bottom-right corner of $(2, 1)$,
</li>

<li>
a segment connecting the top-right corner of $(1, 2)$and the bottom-left corner of $(2, 1)$.
</li>

</ul>

<p>
Thus, Takahashi's score here will be $10+8-2 \times 3=12$.
</p>

<p>
There is no way to mark squares that achieves a strictly higher score, so the answer is $12$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 3 100
1 1 1
1 1 1
1 1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

<p>
It is best to mark no squares.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

8 9 970861213
1313462 943495812 203775264 839015475 115668311 14701110 819458175 827176922 236492592
843915104 786367010 344840288 618248834 824858165 549189141 120648070 805825275 933750119
709330492 38579914 890555497 75314343 238373458 854061807 637519536 53226153 627677130
671706386 380984116 221773266 787763728 639374738 298691145 359138139 183373508 524415106
716502263 150803008 390520954 913021901 553285119 876389099 952721235 46809105 635239775
355621458 511843148 117663063 37274476 891025941 832254337 346436418 783134705 488516288
383723241 322408013 948364423 409068145 120813872 697127655 968230339 988041557 222591780
712959990 233114128 210373172 798667159 568746366 579461421 923556823 777007925 422249456

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

9785518299

</div>

</section>

</div>

</span>

</span>

</div>
