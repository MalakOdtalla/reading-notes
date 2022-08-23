## React

A JavaScript library for building user interfaces

## JSX in React

JSX is a JavaScript Extension Syntax used in React to easily write HTML and JavaScript together.

React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

## Rendering Elements

React element is the smallest renderable unit available in React. We can render such elements using the ReactDOM. React elements are different from DOM elements as React elements are simple javascript objects and are efficient to create. React elements are the building blocks of any React app and should not be confused with React components.

In order to render any element into the Browser DOM, we need to have a container or root DOM element. It is almost a convention to have a div element with the id=”root” or id=”app” to be used as the root DOM element.

React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.

With our knowledge so far, the only way to update the UI is to create a new element, and pass it to root.render().

## Components and Props

Components let us split the UI into independent, reusable pieces, and think about each piece in isolation.

Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

## Handling Events
Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

- React events are named using camelCase, rather than lowercase.
- With JSX you pass a function as the event handler, rather than a string.

See [Reactjs](https://reactjs.org/docs/hello-world.html) full documantation