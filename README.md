# How-to-Talk-Stacks

August 12, 2019

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!

Hire me!

The Stack ADT

A stack is a list with the restriction that insertions and deletions can only be
performed in only one position, namely, the end of the list, called the top.

Stack Model

The fundamental operations on a stack are push, which is equivalent to an insert,
and pop, which deletes the most recently inserted element. The most recently 
inserted element can be examined prior to performing a pop by use of the top
routine. A pop or top on an empty stack is generally considered an error in the 
stack ADT. On the other hand, running out of space when performing a push is an
implementation limit but not an ADT error.

Stacks are sometimes known as LIFO (last in, first out) lists. Pushes are input
operations and pops and tops are output. The usual operations to make empty
stacks and test for emptiness are part of the repertoire, but essentially all 
that you can do to a stack is push and top.

The general model is that there is some element that is at the top of the stack,
and it is the only element that is visible.

Implementation of Stacks

Since a stack is a list, any list implementation will. Clearly list and vector
support stack operations; 99% of the time they are the most reasonable choice.
Occassionally it can be faster to design a special-purpose implementation.
Because stack operations are constant-time operations, this is unlikely to yield
any discernable improvement except under very unique circumstances.

For these special times, we will give two popular stack implementations. One 
uses a linked structure, and the other uses an array, and both simplify the 
logic in vector and list, so we do not provide code.

Linked List Implementation of Stacks

The first implementation of a stack uses a singly linked list. We perform a push
by inserting at the front of the list. We perform a pop by deleting the element
at the front of the list. A top operation merely examines the element at the 
front of the list, returning its value. Sometimes the pop and top operations are
combined into one.

Array Implementation of Stacks

An alternative implementation avoids links and is probably the most popular 
solution. It uses the back, push_back, and pop_back implementation from vector,
so the implementation is trivial. Associated with each stack is theArray and 
topOfStack, which is -1 for an empty stack (this is how an empty stack is
initialized). To push some element x onto the stack, we increment topOfStack and
then set theArray[topOfStack] = x. To pop, we set the return value to 
theArray[topOfStack] and then decrement topOfStack.

Notice that these operations are performed in not only constant time byt very
fast constant time. On some machines, pushes and pops (of integers) can be 
written in one machine instruction, operating on a register with auto-increment
and auto-decrement addressing. The fact that most modern machines have stack
operations as part of the instruction set enforces the idea that the stack is 
probably the most fundamental data structure in computer science, after the
array.

Applications

It should come as no surprise that if we restrict the operations allowed on a 
list, those operations can be performed very quickly. The big surprise, however,
is that the small number of operations left are so powerful and important. We
give three of the many applications of stacks. The third application gives a
deep insight into how programs are organized.

Balancing Symbols

Postfix Expressions

Infix to Postfix Convention
Function Calls

I included some posts for reference.

https://github.com/noey2020/How-to-Talk-Lists-Stacks-and-Queues

https://github.com/noey2020/How-to-Talk-Linear-Regression

https://github.com/noey2020/How-to-Talk-Statistics-Pattern-Recognition-101

https://github.com/noey2020/How-to-Write-SPI-STM32

https://github.com/noey2020/How-to-Write-SysTick-Handler-for-STM32

https://github.com/noey2020/How-to-Write-Subroutines-in-C-Assembly-STM32

https://github.com/noey2020/How-to-Write-Multitasking-STM32

https://github.com/noey2020/How-to-Generate-Triangular-Wave-STM32-DAC

https://github.com/noey2020/How-to-Generate-Sine-Table-LUT

https://github.com/noey2020/How-to-Illustrate-Multiple-Exceptions-

https://github.com/noey2020/How-to-Blink-LED-using-Standard-Peripheral-Library

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!

Hire me!

Have fun and happy coding!
