# Class2 reading

-Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

Render happens first

-What is the very first thing to happen in the lifecycle of React?

the first thing to happen

-Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

1. constructor
2. render
3. componentDidMount
4. react Updates
5. componentwillUnmount

- 

What does componentDidMount do?

## Over all notes

- React allows you to define components as classes or functions, with these classes you are able to use a method on these called "lifecycle events". These can be called during the "lifecycle of a component"... this is where you can update the UI and app. states.

You have 3 phases in a component life cycle :

    -Mounting: This is when an instance of a component is being created/ inserted into the DOM.

     -Updating: Whenever a component is updated or the state changes THEN it gets Rendered, This can happen during updating.

    -Unmounting: This is the final phase, this is when the component is being removed from the DOM.`componentWIllUnmount` the only lifecycle event during this phase.

Before the React component is mounted the `constructor()` is called. If this is in a subclass then use `super(props)`. You can use a constructor to assign state by way of `this.state` (or bind).

*If you use `this.setState()` within a construcor you can get unwanted side effects. One of which would ignore all updates to props... sometimes this is what you want to do, however usually its not what you want*.
  
-`staticgetDerivedStateFromProps()` is a method that is available for use for when "the state" counts on the changing of props.

-`render()` This is the only method that required within a class component. This method examines `thi.props` & `this.state` when it is "called". This function is not meant to change/modify `this` component because it can cause bugs each time the function runs. If the function `shouldCompnentUPdate()` returns false this will make render not be invoked.

-`componentDidMount()` immediately invoked after mounting a component. A good place to add a request a network request or a place to initialize the DOM.

    - `setState()` can be called here. However it will "rerender' so this can mess up the performance.

- `shouldComponentUpdate()` So within react the default is to rerender after every state change. This seeting this to `false` prevents this from happening. This is to keep performance high.

-`getSnapshotBeforeUpdate()` takes picture of DOM to evaluate it before changing anything. 

- `componentDidUpDate()` This performs network requests after a change has happened.

- `componentWillUnmount()` lets you clean up the DOM of requests.

## Video

### What types of things can you pass in the props?

- if you have a counter app your gonna need to intial count inside the props. These are things you are gonna pass to a function.

- you want to display a title and subtitle, then you would want to pass the title and subtitle through the props. this is what you want your function to take. if something in the app changes then the component gets rerendered

### What is the big difference between props and state?

- props you pass into the component state in handled inside thayt  component and props are handled outside that component

intial state gets set to current count ('0')

### When do we re-render our application?

- when the state changes.

### What are some examples of things that we could store in state?

- We could set a counter to '0' and this would set the state to '0' and then the component would render then this data, if the state changes then the state would change and rerender the image.

- Another examlple would be a blank form, the blank form would be rendered via the components and then when the name is added or whatever drop boxes are check then the state would be changed and then so would the state, we would then rerender.

### Two ways to think about data : Props ansd State

- state is there to store or rerender so it acts like memory or "current state" this is when something dynamically changes.

Props: are like an argument to a function, when a component is created and you want it rendered you need to pass the props you want it to have. Props are like a variable to a component

if you have a counter app your gonna need to intial count inside the props.

You are

## Things i want to know more of

- I want to better understand the image that was shown to us on te reading assignment. I can see it but getting it explained to me would be awesome, something is missing.
