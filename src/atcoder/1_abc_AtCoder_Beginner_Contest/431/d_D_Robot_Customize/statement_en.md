
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a robot consisting of a head and a body.
This robot has $N$types of parts that can be attached simultaneously: type $1,$type $2,\ldots,$type $N$.
The weight of the type $i\ (1\le i\le N)$part is $W _ i$.
Each part has a different 
<strong>
happiness
</strong>
when attached to the head versus when attached to the body.
The happiness when the type $i\ (1\le i\le N)$part is attached to the head is $H _ i$, and the happiness when attached to the body is $B _ i$.
</p>

<p>
The robot falls over if the weight of the head is greater than the weight of the body.
Here, the weight of the head and the weight of the body are the sums of the weights of the parts attached to the head or body, respectively.
</p>

<p>
Takahashi wants to attach all $N$types of parts to the robot, one of each.
Find the maximum possible sum of the happiness of all parts when the parts are attached without causing the robot to fall over.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le500$
</li>

<li>
$1\le W _ i\le500\ (1\le i\le N)$
</li>

<li>
$1\le H _ i\le10 ^ 9\ (1\le i\le N)$
</li>

<li>
$1\le B _ i\le10 ^ 9\ (1\le i\le N)$
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

$N$$W _ 1$$H _ 1$$B _ 1$$W _ 2$$H _ 2$$B _ 2$$\vdots$$W _ N$$H _ N$$B _ N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the maximum possible sum of the happiness of all parts when the parts are attached without causing the robot to fall over.
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
1 41 59
2 65 35
8 97 93

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

217

</div>

<p>
By attaching type $1$and type $3$parts to the body and type $2$part to the head, the robot does not fall over and the sum of happiness can be made $217$.
</p>

<p>
It is not possible to attach the parts without causing the robot to fall over and make the sum of happiness $218$or more, so print `217`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1
1 1000000000 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1

</div>

<p>
The robot will fall over if the only part is not attached to the body.
Note that it is acceptable to attach no parts to the head.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

2
1 1000000000 1
1 1 1000000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

2000000000

</div>

<p>
Note that the robot does not fall over if the head and body have equal weights.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

20
483 984529882 299667119
372 428935469 104847758
467 709733529 102461200
421 659244277 110859936
231 786224280 773073478
351 334234040 193222121
119 404159408 772024933
302 519596088 432627257
433 910226244 337833733
184 406236461 530198622
335 465203041 353047747
418 656273464 114923636
482 972364803 329650748
453 748321854 169441643
105 138464898 587159653
401 832952051 506021805
403 810916971 468755944
231 798801044 749313343
292 631278033 556088607
366 567211596 374825770

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

12091388792

</div>

<p>
Note that the answer can exceed $2 ^ {32}$.
</p>

</section>

</div>

</span>

</span>

</div>
