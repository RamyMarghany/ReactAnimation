# React Animation

when we try to animate any element we can normally use the `animation` css property or a `keyframes` css.

but with react these two possibilities are not affective because some react elements not attached to the DOM, so we need to using an additional third part library.

and in this application we are using `react-transition-group`

## This application build by this command

`yarn add react react-transition-group`

## React Transition Group Features

### Transition from "react-transition-group"

it is a component wraps the element that we need to animate it
and has some properties:

- `in` property: using as a flag and receiver the value of the conditional operator for check visibility, and this property is Mandatory.
- `timeout` property: to set how long it takes to switch between animation states and should be equal or less the animation period of the element property is Mandatory.
- `mountOnEnter` property: if in value is true then should add the animated element into the DOM.
- `unmountOnExit` property: if in value is false then should remove the animated element from the DOM.
- `onEnter` apply once the component mount.
- `onEntering` apply directly the component appears.
- `onEntered` after finishing the animation during mounting the element.
- `onExit` apply once the component unmount.
- `onExiting` apply directly the component disappears.
- `onExited` after finishing the animation during unmounting the element.

and the `Transition` component using a callback that return a state to decide the which state to apply a specific animation, and this state return one of four states during mounting/unmounting the element into/from the DOM

- `entering`.
- `entered`.
- `exiting`.
- `exited`.

### CSSTransition from "react-transition-group/CSSTransition"

and this component acting as `Transition` but gives more features related cssClasses, this component has a property calls `classNames` which receive and object of classNames,

### TransitionGroup from "react-transition-group/TransitionGroup"

this component using to apply the animation on a list of element like `ul`, and it has property calls `component`
so simply, replace the `ul` by the `TransitionGroup` and render it as ul by set a value of the component property by ul.

## Relative animation library for react

- React Motion: https://github.com/chenglou/react-motion
- React Move: https://github.com/react-tools/react-move
- Animating Route Animations: https://github.com/maisano/react-router-transition
