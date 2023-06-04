# Lab 5

![Image](lab5.png)

**Instructor Response**

*From the message from the termerinal, your test failed.
Looking by the actual and it's expected results, the program did
sort the integers, however it's in descending order. 
This means the problem is occuring where your code is indentifying 
which integers are greator and less than your pivot. 
Look back at the logic of those methods*


**FIX

![Image](lab5fix.png)

*The bug ended up being a logical error in the way the arrays were being partitioned.
By using > instead of < when attemping to find elements smaller than the pivot and
< instead of > for elements larger than the pivot the code incorrectly identifies the elements 
greater than the pivot as smaller and vice versa. As a result, the sorting order is reversed,
leading to incorrect sorting of the elements.*
