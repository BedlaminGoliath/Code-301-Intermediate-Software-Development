# Class 4 Reading Notes

## What is a ‘Controlled Component’?

So within React the state of a form is usually kept within the `state property` of the components, "... and is usually updated with `setState()`. In react, we are able to make the react state the "...single source of truth  ". Reacts components that render the form can also control what the forms data renders, upon user input. We can create a form element that acts as a shell that holds the users input.

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why

I think being able to update and store as  the user types is a good way to handle the data. This way we are able to store what is being put in and this would not take up as much memory by constantly storing the info. Once it is submitted then we could store it in state.

## How do we target what the user is entering if we have an event handler on an input field?

We can use the `name` attribute to each of ther elements that way the handler function can chose what to do "based on the value of the `event.target.name`".

## notes on forms

-forms in React keep some form of state.
-In standard HTML `<input>`, `<textatrea>` and `<select>` typically maintain their own state.
while using the `select` element (which creates a drop down menu). In HTML we would creat a `selected value` attribute in order to start of that item as the "checked item" however in React we are able to use a  `value` attribute on the select tag.

## Ternary

## Why would we use a ternary operator?

We could use ternary, While we are working with conditionals that offer a value to an object we are working on. This way we can update our property in our object according to a users input, there for this could "unlock"certain alerts or features that would only be avaible is a condition is met.

## Rewrite the following statement using a ternary statement

`if(x===Y){
    console.log(true);
}else{
    console.log(fale);
}`

`if x === y ? console.log(true): console.log(false)`

## Notes on Ternary Ops

The ternary is another one like way to write out our classic `if` statement`

The basic format is:
`condition ? value if true : value if false`

What we need to know is: the condition we are testing And the result needs to be either true or false or a boolean of some sort. Next we would place what would happen "if true" between the `?` and the `:` (this is what is executed if  the statement is true). After the colon we would write out what would happen if the condition is false.
