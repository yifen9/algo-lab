
<div>

<span>

<span>

<p>
Score : $250$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<p>
You are trying to implement collision detection in a 3D game.
</p>

</blockquote>

<p>
In a $3$-dimensional space, let $C(a,b,c,d,e,f)$denote the cuboid with a diagonal connecting $(a,b,c)$and $(d,e,f)$, and with all faces parallel to the $xy$-plane, $yz$-plane, or $zx$-plane.

(This definition uniquely determines $C(a,b,c,d,e,f)$.)
</p>

<p>
Given two cuboids $C(a,b,c,d,e,f)$and $C(g,h,i,j,k,l)$, determine whether their intersection has a positive volume.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$0 \leq a < d \leq 1000$
</li>

<li>
$0 \leq b < e \leq 1000$
</li>

<li>
$0 \leq c < f \leq 1000$
</li>

<li>
$0 \leq g < j \leq 1000$
</li>

<li>
$0 \leq h < k \leq 1000$
</li>

<li>
$0 \leq i < l \leq 1000$
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
The input is given from Standard Input in the following format:
</p>

<div>

$a$$b$$c$$d$$e$$f$$g$$h$$i$$j$$k$$l$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print `Yes`if the intersection of the two cuboids has a positive volume, and `No`otherwise.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

0 0 0 4 5 6
2 3 4 5 6 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes

</div>

<p>
The positional relationship of the two cuboids is shown in the figure below, and their intersection has a volume of $8$.
</p>

<p>

<img src="https://img.atcoder.jp/abc361/12ad1f07f2801946704198807bbb3395.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

0 0 0 2 2 2
0 0 2 2 2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No

</div>

<p>
The two cuboids touch at a face, where the volume of the intersection is $0$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

0 0 0 1000 1000 1000
10 10 10 100 100 100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

Yes

</div>

</section>

</div>

</span>

</span>

</div>
