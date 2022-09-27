# Notes for class 3

## List and keys

## What does .map() return?

This returns a "new array" of altered items as defined within the `.map()` method.

## If I want to loop through an array and display each value in JSX, how do I do that in React?

- In this example we were shown that you can use the `.map()` method. within the parens of the method we create a method that assigns the items to a `<li>` from there we take that `return` from there we input that info into a a render component where it should get displayed.

- a *key* is a string attrbute that is required when creating a list of elements.

- The use of the the *key* attribute. takes place inside of the function that takes place within the `.map()` method. This affects what is taking place within th method itself.

- Its important to note that you do need to use the `{}` to leave html land and head over to jsx land.

``function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>``

   ``<li key={number.toString()}>
      {number}
    </li>
  );
  return (
    <ul>{listItems}</ul>
  );
}``

within the example above you can see that withing the function we and within the `li` element we use the attribute `key` we open with curly braces. here we place what is being effected in this context its the `number` array and it is being changed from an array over to a string (i assume.)

## Each list item needs a unique ____

This is asking to use a unique ID That " identifies the list item among ts siblings...." (taken from [react.js](react info). If the special Id is not given then by default react will go with the indexes of said elements however this becomes a problem if the order of these elements change.

Keys within arrays should be unique in the context of their scope. each array can have its own key and that key can be used within the context of an new array. Unique amongst their siblings.

## What is the purpose of a key?

## overall notes

Keys dont get passed through componenets. If the same value is needed then pass as a prop.

## Spread Op

## What is the spread operator?

A spread operator adds items into arrays or can combine array. The spreads the array into seperate arguments.

## List 4 things that the spread operator can do

the spread operator can free you up to input an array as an argument within certain function `Math.max()` you cannot put an array directly into this function however leading with `...` makes it okay. A few other uses is to :

- Copy and array

- when you use math functions

- concatenating or combing an array

- when you use an array as an argument.

## Give an example of using the spread operator to combine two arrays

## Give an example of using the spread operator to add a new item to an array

## Give an example of using the spread operator to combine two objects into one

you cant use an array as an arguement withing the `Math.max(1,3,4);`

however in order to make this happen you could add the spread operator before you put in the array... as an array. because simply putting the array within the parens as an arguement does not work.

## video

## In the video, what is the first step that the developer does to pass functions between components?

They create a function where the state is that we want to change. He then uses the `.map()` method to iterate through an array.

## In your own words, what does the increment function do?

The increment function iterates through the array of objects, the array of people are held in state with their count as '0'. So this functions is gonna use the `.map()` method to check if the name of the "person" matches the name of people and then increment the "count" state buy one.They then take the return it.

## How can you pass a method from a parent component into a child component?

you need to create a function where the state is. since the state is usually placed in a place where the method is accessible.

## How does the child component invoke a method that was passed to it from a parent component?

You would pass it like you would a prop but it is a method that was created within the component however you would use `this.props.methName`.
