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

## Things i want to know more of

- I want to better understand the image that was shown to us on te reading assignment. I can see it but getting it explained to me would be awesome, something is missing.
