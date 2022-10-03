# Class 5 Reading

## What is the single responsibility principle and how does it apply to components?

This is the idea That a component should only be responsible for doing **one thing**. At point in the article they even discuss the naming convention and how it could be the name of the file used in the photoshop process. Understandibly so If a component starts to expand and becomne something too big than it may be time to break it down into smaller 'subcomponents'.

## What does it mean to build a ‘static’ version of your application?

A static version of the app is having an app that is the structure and no ability to interact. This way You can focus on building your components and placing them where they need to be. This is helpful because this takes little brain power (logic) so you can focus on this aspect, the components will render and you can see it layed out.. once this is done then you can move onto the functional aspect of your app.

## Once you have a static application, what do you need to add?

The next big part of this is seeing what is being passed in as props and what is being stored in state. This helps to see what is going to be actually changed via the user input and what is going to remain a simple component pased via props

## What are the three questions you can ask to determine if something is state?

Is it passed in from a parent via props? If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.
Can you compute it based on any other state or props in your component? If so, it isn’t state.

[taken-from-react.com](https://reactjs.org/docs/thinking-in-react.html)

## How can you identify where state needs to live?

In order to find who owns state it is good practice to find which components will be mutated (altered) during (commonly) user input, you would then place the state within the parent element of the component(components) that would be changed. If you cannot find a single parent component that is over seeing the change than you can always create a parent component that will handle its children.

## overall notes and resources

For each piece of state in your application:

Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Higher -Order Functions

## What is a “higher-order function”?

Higher order functions are functions that "opperate" on other functions (by taking them in as arguments or by returning them). Since we are able to return functions or even understand them as a value then it is not unusualy to be able to apply those values to other functions. This is where the concept of abstraction comes into play. Where are able to not get too into the details and utilize the input and or output and apply those to another function.

## Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

The `greaterThan()` function seems to be a function that takes in a parameter `n` (as an argument). It then is returning an anonymous functions that takes in a parameter `m` and checks if `m` is > `n`.

In the context of the example: It is a function that takes in the intial "base number"(10), it then returns a function that takes in another paramter 'm' (in this case its 11) and checks if 11 is greater than 10.

## Explain how either map or reduce operates, with regards to higher-order functions

So from what I understand is we are creating a function called "map" that takes in an array and transform argument.
within the code block we create a new empty array.
beneath that we are using a `for...of` statement that iterates through each element of the aray and then we are pushing the 'transformed(the function that was a argument inside the map function) THAT takes in the specific element we are iterating over and then THAT gets pushed nto the empty array.

## Things I want to know more about

I want to hear the example in the reading explained... I think I can kind of understand it but its something I will have to revisit.

``function map(array, transform) {
  let mapped = [];
  for (let element of array) {
    mapped.push(transform(element));
  }
  return mapped;
}

let rtlScripts = SCRIPTS.filter(s => s.direction == "rtl");
console.log(map(rtlScripts, s => s.name));
// → ["Adlam", "Arabic", "Imperial Aramaic", …]
``
