# Class 10 Reading

## What is a ‘call’?

A function invocation.

## How many ‘calls’ can happen at once?

One at a time from top to bottom. (synchronous).

## What does LIFO mean?

Last In First Out.

## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack

( I dont understand it that much yet).

## What causes a Stack Overflow?

This happens when we have a function that calls itself and there is no return (exit point). The Browswer has a certain amount of stack calls that it can handle before getting angry. Oncen it throws the error THAT is when we have a stack overflow.

## overall notes

A callstack is a data structure that uses LIFO which is used to temporarily store and manage function calls.

### Error Messages

## What is a ‘reference error’?

This usually happens when you try to use a variable that has not yet been declared.

This is usually fixed by declaring the var before any declaration is made.

## What is a ‘syntax error’?

This is self descriptive. This usually happens due to a syntax error.

## What is a ‘range error’?

This happens when you try to manipulate an array with some length that is invalid because THAT length isnt even a thing.

## What is a ‘type error’?

This usually happens when the "types" (number, string...) you are trying to use or access are not compatible. like trying to access a property in an object that is not defined.

(this is likely the most common error in js).

## What is a breakpoint?

A break point is a point in your code that will act like a stopsign and will halt at that moment that way you can begin to isolate the break code block, you can also use conditional break points. This also gives you the power to move line by line. 

## What does the word ‘debugger’ do in your code?

This allows you to see the "history" of what is happening instead of looking at a massive call stack at the end, this way you are able to trace each code blocks problem (or not a problem)

### Things I want to know more about

 I want to understand this enough to be able to answer the question about drawing an example. I can picture what is going on but i dont know how to explain that.,

### overall notes2

reference errors often happen to const and let this is called Temporal Dead Zone.