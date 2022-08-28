# React

## Conditional Rendering

In React, conditional rendering refers to the process of delivering elements and components based on certain conditions.

## Lists and Keys

React  simplifies the rendering of lists inside the JSX by supporting the Javascript .map() method, it iterates through the parent array and calls a function on every element of that array. Then it creates a new array with transformed values. It doesn’t change the parent array. And key is kind of the id for the element, and it helps React to identify which element was changed, added, or removed.

## Forms

React uses forms to allow users to interact with the web page.HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.

## Lifting State Up

Lifting state up is a common pattern that helps avoid more complex (and often unnecessary) patterns for managing state.

## Composition vs Inheritance

 When a child class derives properties from it’s parent class, we call it inheritance.
 Composition is a familiar concept in Object Oriented Programming. Instead of inheriting properties from a base class, it describes a class that can reference one or more objects of another class as instances.

## Thinking in React
Here are four concepts that should help developer think clearer when it comes to creating next React component.

Step 1: Break The UI Into A Component Hierarchy

The easiest way to determine this is to apply a single responsibility rule. What this means is that a component should only do one thing. Any time a component grows larger than a single responsibility, it should be refactored and decomposed into a collection of smaller components.


Step 2: Build A Static Version in React

When building  UI, it can be tempting to code each individual component as separate parts and put them all together. This can be a logistic issue, especially on the CSS front, when it comes to getting things to sit in the right places for different view ratios.

This is why it's good to start with a static version that renders the entire view first. A static version just consumes the data and presents it on the screen. It doesn't matter in which order  begin constructing  UI.  main focus here is to fit all the pieces together at the visual level.
To build a static version of the app that renders data model, developer need to build components that reuse other components and pass data using props.

Step 3: Identify The Minimal (but complete) Representation Of UI State

It is when a developer is able to capture wholly the minimum required states for your entire application. This means that you're not repeating yourself in another component. If you find yourself typing the same code (or something similar), it means that you are creating duplicates and not applying DRY on your code.

Step 4: Identify Where Your State Should Live

React uses one-way data flow down the hierarchy. This means that children can only consume the data and are unable to enact any changes. Figuring out where a state should live is a process of determining what component is the parent in the hierarchy.

Here are a few simple steps that developer can follow:

- Identify every component that renders something based on that state.
- Find a common owner component or a single component that exists above all the components that need the state in the hierarchy – i.e. the parent. This is the component that should own the state.
- If there is no component that makes sense for owning the state. Create a new component just for holding the state and keep it separate until a logical component comes into existence that sits above the common components.