# RTS
RTS Problem solving applications

Topics and formulas

From video 10 Onwards..

-----------------------------------------------------------------------------------------------------------------------------------

Schedulable Utilization of Rate Monotonic Algorithm (RM)

The case in which Deadline (Dk) is not equal to period. We will assume the deadline is some multiple 'v' of the period


**Dk = v.Pk** 

Here 'Dk' is relative deadline.
'p' is the multiple factor.
'Pk' is the period of respective task.


**So for 0 <= v <= 0.5, 			Urm (n,v)  =  v**     			   		 

**So for 0.5 <= v <= 1, 			Urm (n,v)  =    n((2v)^(1/n) -1)+1-v**      		

**So for v = 2,3,4,5......integer, 	Urm (n,v)  =    v(n-1)[(((v+1)/v)^((1/n)-1)) - 1 ]**      


Note:- This method is only applicable if the ratio (v) is same for all task. Also it is not aplicable when value of v will be fractional numbers greater than 1. i.e 1.5,2.5 ......


Lets have an example to understand when it will not be applicable..............

T1(4,1) T2(4,1,6) T3(5,1,10)

Now for T1(4,1)

D1 = 4
P1 = 4

v1 = D1/P1 = 4/4 = 1;

Now for T2(4,1,6)
 
D2 = 6
P2 = 4 

v2 = D2/P2 = 4/6 = 1.5;

Now for T3(5,1,10)
 
D3 = 10
P3 = 5 

v3 = D3/P3 = 10/5 = 2;

Here v1 != v2 != v3 ; So above  method will not be applicable in this problem statement.

------------------------------------------------------------------------------------------------------------------------------------

Two term are coined here 

optimality & schedulability of an Algorithm.



