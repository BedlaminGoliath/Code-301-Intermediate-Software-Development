# Class 9 Reading

## What is functional programming?

Functional programming is primarliy using functions to structure your code. This is where we are using higher order functions to play our arguments which come from functions and we continue the trend with the output.

This would mean that the functions are staying "true to state" as opposed to dealing with variables where we would be changing the state.

## What is a pure function and how do we know if something is a pure function?

It will always return the same result as long as the arguements are consistantly the same. We would know if we tested the function by giving it the same in put time and time again and recieved the same output.

` An impure function would receive radius as the parameter, and then calculate radius * radius * PI: ` (medium.com).

I believe this has to do with the "flucuation" of the input (in this instance its `pi` which some could argue equals another number... because PI has caused wars). And because It used a global object that "...was not passed as a parameter to the function."

If our function reads external files, its not a pure function.... because the files content can change..

## What are the benefits of a pure function?

This should make for code that is easier to test.

## What is immutability?

This means that the data (datas state) that is immutable cannot be changed after it has been created. However, if you do want to change the data you wouldnt... you would have to create a new object with the new value.

## What is Referential transparency?

When a function yeilds the same result for the input it is referentially transparent.

`pure function + immutable data = referential transparency`

## Node.js

## What is a module?

This is a single function that is organized in a single (or several) files which can be reused throught the node.
This seperates the functionatilty and allows us to split up the function.

## What does the word ‘require’ do?

require is like an "import". This is a global object. we place the path that we will require to "attach" our modules together.

## How do we bring another module into the file the we are working in?

after we export the module the current working module we are supposed to "import" the module into our other file, but that is not enough we need to reference that method by way of assigning the function to a variable and that way we can reference that function inside our new module.

## What do we have to do to make a module available?

 we assign the `require()` to a varible that way we can use that variable as a method

### definitions and concepts

keep functions seperate.

functions are treated as first class citizens.

We isolate our function therefore we are unable to affect other parts of our code. Because we are not modifying the global objects and or variable.

we handle mutability in iteration via "recursion". With recursion we keep our vairiables immutable.

function chaining = function composition.

## things I want to know more about

I want to better understand what an impure function is.
