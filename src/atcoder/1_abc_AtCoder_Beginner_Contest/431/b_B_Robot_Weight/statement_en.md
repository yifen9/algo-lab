
<div>

<span>

<span>

<p>
Score : $200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a robot, and initially the weight of the robot is $X$.
This robot has $N$types of parts that can be attached simultaneously: type $1,$type $2,\ldots,$type $N$.
The weight of the type $i\ (1\le i\le N)$part is $W _ i$.
Initially, none of the $N$types of parts are attached to the robot.
</p>

<p>
Process the following $Q$queries in order.
The $i$-th query $(1\le i\le Q)$is represented by an integer $P _ i$and is as follows:
</p>

<ul>

<li>
If the type $P _ i$part is not currently attached to the robot, attach it; if it is attached, remove it. Then, print the current weight of the robot.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le X\le100$
</li>

<li>
$1\le N\le100$
</li>

<li>
$1\le W _ i\le100\ (1\le i\le N)$
</li>

<li>
$1\le Q\le100$
</li>

<li>
$1\le P _ i\le N\ (1\le i\le Q)$
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

$X$$N$$W _ 1$$W _ 2$$\ldots$$W _ N$$Q$$P _ 1$$P _ 2$$\vdots$$P _ Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.
The $i$-th line $(1\le i\le Q)$should contain the result of processing the $i$-th query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

31
4
15 92 65 35
4
3
1
4
1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

96
111
146
131

</div>

<p>
Initially, the weight of the robot is $31$.
For each query, the weight of the robot becomes as follows:
</p>

<ul>

<li>
In the $1$-st query, attach the type $3$part to the robot. The weight of the robot becomes $31+65=96$.
</li>

<li>
In the $2$-nd query, attach the type $1$part to the robot. The weight of the robot becomes $96+15=111$.
</li>

<li>
In the $3$-rd query, attach the type $4$part to the robot. The weight of the robot becomes $111+35=146$.
</li>

<li>
In the $4$-th query, remove the type $1$part from the robot. The weight of the robot becomes $146-15=131$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

41
10
73 8 55 26 97 48 37 47 35 55
15
1
2
7
1
6
3
10
8
4
8
1
5
9
9
3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

114
122
159
86
134
189
244
291
317
270
343
440
475
440
385

</div>

</section>

</div>

</span>

</span>

</div>
