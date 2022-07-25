# Instructions

LOAD: 
```
 > 
-->
 > 
```
Takes a value, and adds it to the end of the queue.

STORE:
```
 <
<--
 <
```
pops the first item from the queue and stores it at the memory adress passed to it.

MUL/DIV/ADD/SUB:
```
* *
 * 
* *
  /
 /
/
 +
+++
 +

---

```
Multiplies/Divides/Adds/Subtracts the first 2 items in the queue, and overwrites it with the result.

PUT:
```
@->
@->
@->
```
pops the first item from the queue, and prints it to standard output.

LABEL:
```
|-|
|*|
|-|
```
here \* repersents a wildcard for any value 0-16. defines a label that can be jumped to

GotoEq:
```
@->
@*>
@->
```
here \* repersents a wildcard for any value 0-16. jumps to the label with that value if the value passed is equal to the first value in the queue.

GotoNeq:
```
@->
!*>
@->
```
here \* repersents a wildcard for any value 0-16. jumps to the label with that value if the value passed is *not* equal to the first value in the queue.
