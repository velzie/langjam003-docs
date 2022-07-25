# Syntax

The syntax of x86-art is extremely simple. Each "line" consists of an instruction, and optionally a value passed.

Each instruction is a 3x3 block of text, 3 lines down and 3 characters across. For example, this is the MUL instruction
```
* *
 * 
* *
```
Some instructions require an value passed to them, such as the LOAD instrution
```
 > ***
-->*2*
 > ***
```
The number inside the asterisks can be any single digit hex value. In this case it is 2. This will result in the value of 2 being added to the queue
There are 2 kinds of values. The example above shows the literal value 2 being added. If you instead would run this line
```
 > @@@
-->@2@
 > @@@
```
It would instead look up whatever value is at location 2 in memory, and add that to the queue
Note that there is no space between the instruction and the value. adding a space will cause the program to crash

Comments are made by making a new line starting with `;`
If you have a empty new line not starting with `;`, it will attempt to use that as an instruction and crash

Some instructions, like LABEL and GOTO are repersented like this
```
|-|
|0|
|-|
```
The `0` can be changed to any other value and it will mark that as the label