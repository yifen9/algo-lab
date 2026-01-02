
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
The Christmas season this year is over, and it is finally time for the new year. Takahashi is busy with the big cleanup of putting away the Christmas tree.
</p>

<p>
There is a Christmas tree decorated with bulbs in three colors: red, blue, and green. The Christmas tree has $N$bulbs, and they are connected by $N-1$ribbons. When viewing the bulbs as vertices and the ribbons as edges, this graph is a tree.
</p>

<p>
The bulbs are numbered from $1$to $N$, and the ribbons are numbered from $1$to $N-1$. Ribbon $i$connects bulbs $u_i$and $v_i$. Bulb $i$is initially lit in red if $c_i$is `R`, in green if it is `G`, and in blue if it is `B`.
</p>

<p>
Takahashi is considering performing the following operation $N-1$times to remove all ribbons.
</p>

<ol>

<li>
Choose one ribbon among those not yet removed where the bulbs at both ends have different colors, and remove that ribbon.
</li>

<li>
Let bulbs $u$and $v$be the bulbs at both ends of the removed ribbon. For each of the bulbs $u$and $v$, change the color they are lit in according to the following rule:
<ul>

<li>
If it was lit in red, light it in green.
</li>

<li>
If it was lit in green, light it in blue.
</li>

<li>
If it was lit in blue, light it in red.
</li>

</ul>

</li>

</ol>

<p>
Determine whether it is possible for Takahashi to remove all ribbons by repeating this operation. If possible, output one such method.
</p>

<p>
You are given $T$test cases. Solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq T\leq 20000$
</li>

<li>
$2\leq N\leq 2000$
</li>

<li>
$c_i$is `R`, `G`, or `B`.
</li>

<li>
$1\leq u_i,v_i\leq N$
</li>

<li>
When viewing the bulbs as vertices and the ribbons as edges, the given graph is a tree.
</li>

<li>
$T,N,u_i,v_i$are integers.
</li>

<li>
The sum of $N^2$in one input file is at most $2000^2$.
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$c_1c_2\ldots c_N$$u_1$$v_1$$u_2$$v_2$$\vdots$$u_{N-1}$$v_{N-1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for $\mathrm{case}_1, \mathrm{case}_2, \ldots, \mathrm{case}_T$in order in the following format.
</p>

<p>
If it is impossible to remove all ribbons, output `No`.
</p>

<p>
If it is possible, let $e_i$be the number of the ribbon removed in the $i$-th operation, and output:
</p>

<div>

Yes
$e_1$$e_2$$\ldots$$e_{N-1}$
</div>

<p>
$(e_1, e_2, \ldots, e_{N-1})$must be a permutation of $(1, 2, \ldots, N-1)$.
</p>

<p>
If there are multiple solutions, any of them will be accepted as correct.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
4
GBBR
1 2
1 3
1 4
3
RRR
1 2
2 3
5
RGBRG
1 2
2 3
3 4
3 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
1 3 2
No
Yes
1 4 2 3

</div>

<p>
For the first test case, for example, all ribbons can be removed by performing the operations as follows:
</p>

<ul>

<li>
Initially, the colors of the bulbs are green, blue, blue, red, in order (from bulb $1$).
</li>

<li>
Remove ribbon $1$. After removal, the colors of the bulbs are blue, red, blue, red, in order.
</li>

<li>
Remove ribbon $3$. After removal, the colors of the bulbs are red, red, blue, green, in order.
</li>

<li>
Remove ribbon $2$. After removal, the colors of the bulbs are green, red, red, green, in order.
</li>

</ul>

<p>
The $(e_1, e_2, e_3)$satisfying the condition are $(1, 3, 2)$and $(2, 3, 1)$, and either one will be accepted as correct.
</p>

<p>
For the second test case, it is impossible to remove all ribbons no matter how you perform the operations.
</p>

</section>

</div>

</span>

</span>

</div>
