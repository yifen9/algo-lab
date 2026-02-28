
<div>

<span>

<span>

<p>
Score : $625$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Snuke is choosing problems to use in programming contests he is hosting.
Snuke has $N$problem candidates numbered $1$to $N$, where problem candidate $i$has 
<strong>
difficulty
</strong>
$i$, 
<strong>
genre
</strong>
$K_i$, and 
<strong>
interest
</strong>
$A_i$.
</p>

<p>
Hoping to entertain participants of a wider range of skill levels, he plans to simultaneously hold two contests called 
<strong>
Div. 1
</strong>
and 
<strong>
Div. 2
</strong>
, each featuring four problems chosen from the $N$problem candidates with 
<strong>
pairwise distinct genres
</strong>
.
However, to conserve problem candidates, the two easier problems in Div. 1 and the two harder problems in Div. 2 will be the same, so only six problems in total will be used.
</p>

<p>
More formally, the following holds:
</p>

<ul>

<li>
Snuke chooses six problem candidates from the $N$candidates. Let the numbers of the chosen problem candidates in ascending order be $i_1, i_2, \dots, i_6$.
</li>

<li>
Problem candidates $i_1, i_2, i_3, i_4$are used in Div. 2, and they must be of pairwise distinct genres. That is, $K_{i_1}, K_{i_2}, K_{i_3}, K_{i_4}$must be pairwise distinct.
</li>

<li>
Problem candidates $i_3, i_4, i_5, i_6$are used in Div. 1, and they must be of pairwise distinct genres. That is, $K_{i_3}, K_{i_4}, K_{i_5}, K_{i_6}$must be pairwise distinct.
</li>

</ul>

<p>
Determine whether there exists a valid choice of six problems satisfying the conditions, and if so, find the maximum total interest of the six chosen problems.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$6 \leq N \leq 10^5$
</li>

<li>
$1 \leq K_i \leq N$
</li>

<li>
$1 \leq A_i \leq 10^9$
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

$N$$K_1$$A_1$$K_2$$A_2$$\vdots$$K_N$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If there exists a valid choice of six problems satisfying the conditions, output the maximum total interest of the six chosen problems; otherwise, output `-1`.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

8
1 9
3 4
2 3
1 5
4 6
3 3
4 1
5 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

32

</div>

<p>
For example, consider choosing problem candidates $1, 2, 3, 5, 6, 8$.
In this case, $K_{i_1}=1, K_{i_2}=3, K_{i_3}=2, K_{i_4}=4$are pairwise distinct, and $K_{i_3}=2, K_{i_4}=4, K_{i_5}=3, K_{i_6}=5$are also pairwise distinct, so this is a valid choice.
The total interest in this case is $9+4+3+6+3+7=32$, which is the maximum.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

7
1 1
2 1
1 1
3 1
4 1
2 1
3 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1

</div>

<p>
There is no valid choice of six problems satisfying the conditions.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

16
1 593
3 449
15 991
9 310
1 355
15 68
3 431
15 580
14 757
14 218
14 934
9 328
3 676
3 355
1 221
6 80

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

3971

</div>

</section>

</div>

</span>

</span>

</div>
