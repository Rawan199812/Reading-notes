## React 1

***React is a JavaScript library, and so we’ll assume you have a basic understanding of the JavaScript language. If you don’t feel very confident, we recommend going through a JavaScript tutorial to check your knowledge level and enable you to follow along this guide without getting lost.***

**JSX**

**JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.**
**React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.**

### Rendering an Element into the DOM

**Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.**


### Updating the Rendered Element

**React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.**

### React Only Updates What’s Necessary

**React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.**


### Rendering a Component

**When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object “props”.**

- We call ReactDOM.render() with the <Welcome name="Sara" /> element.
- React calls the Welcome component with {name: 'Sara'} as the props.
- Our Welcome component returns a <h1>Hello, Sara</h1> element as the result.
- React DOM efficiently updates the DOM to match <h1>Hello, Sara</h1>.

**All React components must act like pure functions with respect to their props.**

***In React apps, whether a component is stateful or stateless is considered an implementation detail of the component that may change over time. You can use stateless components inside stateful components, and vice versa.***

**Handling events with React elements is very similar to handling events on DOM elements.**

**When using React, you generally don’t need to call addEventListener to add listeners to a DOM element after it is created. Instead, just provide a listener when the element is initially rendered.**

**If you refer to a method without () after it, such as onClick={this.handleClick}, you should bind that method.**



## Next.js: The React Framework

**Enter Next.js, the React Framework. Next.js provides a solution to all of the above problems. But more importantly, it puts you and your team in the pit of success when building React applications.**

- Next.js has the best-in-class "Developer Experience" and many built-in features.

**A framework can solve these problems. But such a framework must have the right level of abstraction — otherwise it won’t be very useful. It also needs to have great "Developer Experience", ensuring you and your team have an amazing experience while writing code.**


