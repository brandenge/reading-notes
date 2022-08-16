# React State and Props

### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

render.

### What is the very first thing to happen in the lifecycle of React?

The constructor is invoked to create a new component.

### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

1) constructor
2) render
3) React Updates
4) componentDidMount
5) componentWillUnmount

### What does componentDidMount do?

It returns true or false, confirming whether a component did mount or not. This is useful for notifying other parts of the system if needed when a component is mounted.
