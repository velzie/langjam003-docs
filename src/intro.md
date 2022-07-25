# Introduction

Hello! this is the documentation website for my entry into langjam003, x86-art. You can view its source code [here](https://github.com/langjam/jam0003/tree/main/x86-art) although you may not like what you see

x86-art is an interpreter for my custom instruction set, consisting of only 10 instructions.

There are examples on how to use the program in the /examples directory in the source code

It has only 16 memory slots, where each slot can hold a value from 0 - 16
However, it also has a queue, that can hold an infinite amount of values.

It's worth mentioning that there is zero concept of error handling. If you do anything wrong, the program will instantly panic and leave you with no indication of what exactly went wrong. I ran out of time to add error messages.