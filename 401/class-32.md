## React 2 

**Forms**

**HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.** 

**Controlled Components**
***In HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().***

**The textarea Tag**

In React, a <textarea> uses a value attribute instead. This way, a form using a <textarea> can be written very similarly to a form that uses a single-line input

**The select Tag**
***React, instead of using this selected attribute, uses a value attribute on the root select tag. This is more convenient in a controlled component because we only need to update it in one place.***


- To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.

- To make UI interactive, you need to be able to trigger changes to the underlying data model. React achieves this with state.

**Lists and Keys**

- In React, transforming arrays into lists of elements is nearly identical.

***Rendering Multiple Components*** we can build collections of elements and include them in JSX using curly braces {}

One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React.


- To build the app correctly, you first need to think of the minimal set of mutable state that your app needs. The key here is DRY: Don’t Repeat Yourself. Figure out the absolute minimal representation of the state the  application needs and compute everything else you need on-demand. For example, if you’re building a TODO list, keep an array of the TODO items around; don’t keep a separate state variable for the count. Instead, when you want to render the TODO count, take the length of the TODO items array.