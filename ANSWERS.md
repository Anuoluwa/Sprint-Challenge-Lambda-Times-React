- [x] What are PropTypes used for? Please describe why it's important to type check our data in JavaScript.

PropTypes ensure that the right type of props is passed to a component — and, conversely, that the receiving component is receiving the right type of props.
PropTypes would ensure that the correct object is being passed and that it is passed to the correct receiver.

- [ ] Describe a life-cycle event in React?

You can think of the lifecycle in react as a simple set of phases in a component’s life: Birth/Mounting, Growth/Updating and Death/Unmounting

The Birth/Mounting Phase
This is the phase when the component is being built out from ground up.
Whatever initial data you’ll have access to will be defined on the constructor of this phase
Your render method is invoked.
componentDidMount gets called as well.

Growth/Updating Phase
setState can be used to change the component’s state data, forcing a call to render.
shouldComponentUpdate is a method one could use here to stop a component from calling render if necessary.

Death/Un-mounting Phase
Component is removed from the screen.
componentWillUnmount is called and can be used for any clean up you may need to do.


- [x] Explain the details of a Higher Order Component?

A higher-order component (HOC) is an advanced technique in React for reusing component logic. They are a pattern that emerges from React’s compositional nature. in a way higher-order component is a function that takes a component and returns a new component.

- [ ] What are three different ways to style components in React? Explain some of the benefits of each.

a. Inline styling
b. External CSS sheets
c. Style Components 

a. Inline styling: There is no need to upload multiple files. HTML and CSS can be in the same file, there no http requests.
Only one page is affected by stylesheet.

b. External CSS sheets:
    - Smaller size of HTML pages and cleaner structure.
    - Faster loading speed.
    - Same .css file can be used on multiple pages.

c. Style Components 
    - With styled-components, the user interface design focus shifts from just merely styling HTML elements or React components through className to defining styled components that contain their own styles and are so easily reusable across the entire project
    - One the benefits of Styled Components is that external CSS files are global in scope and always leak in the entire codebase, therfore not helpful in scaling apps
