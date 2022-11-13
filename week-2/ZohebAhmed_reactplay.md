Link to the Article => https://aviyel.com/post/3844/what-are-react-hooks-anyway

# Introduction

[Hooks](https://reactjs.org/docs/hooks-intro.html) are a recent addition to [React 16.8](https://reactjs.org/blog/2019/02/06/react-v16.8.0.html). As per the official [documentation](https://reactjs.org/docs/hooks-intro.html), Hooks let you use state and other features of React without going through the trouble of writing a class.

# But why call it "hooks"?

Well, that’s because the react hooks are very similar to the fishing hooks, which help the person holding the fishing rod to catch the fish in the sea. Very similar to that, react hooks are functions that allow you to "hook into" react state and lifecycle features.

However, unlike the lifecycle methods, the react hooks cannot be used inside classes. This, in fact, makes our job much easier by letting us use lifecycle methods directly from the function components.

So basically, hooks allow [React functional components](https://reactjs.org/docs/hooks-overview.html) to use React features that were previously only made available in [React class components](https://www.w3schools.com/react/react_class.asp), thereby providing us with a cleaner way to combine them.

# But how exactly are react "hooks" helpful?

When react hooks were not introduced, the functional components and class components were used to perform two different functions.

The functional components were only used to extend the data to the interface of the application. Functional components were only capable of getting props from the class-based components and then rendering them to the UI. These components did not have the ability to interfere with the state and had no clue about the lifecycle methods.

On the contrary, class-based components were responsible for keeping track of the applications’ internal state and performing operations during each phase by making use of lifecycle methods. These components were responsible for operations like fetching and updating data once the components were mounted.

But then came the hooks, which solved the problem by giving functional components the ability to manage the internal state and lifecycle. Apart from this, it also solved a number of unconnected problems in react. Let’s look into the other problems solved by react hooks.

## **Clearing "this" up:**

In class-based components, every time we render a state to the UI or call a method, we have to bind each of the states individually by using the "this" keyword. And on top of that, we have the extra syntax of calling the super(props) in the default constructor.

![image](https://user-images.githubusercontent.com/75200954/201414387-c029a33e-379b-46b5-89f7-d94ac4025065.png)

But now, with functional components, we do not need a constructor. We can simply import the `useState()` hook and create a state, initialize it and update it without binding it every time with the "this" keyword. The useState hook takes in only one argument and returns an array with two values, the first one being the current state and the second one being a function allowing us to update the value of the state.

## **Too much syntax**

Class-based components have innumerable syntaxes involved, which increases the length of your component by splitting the overall logic of the component into different lifecycle methods like `componentDidMount()`, `componentDidUnmount()`, `componentDidUpdate()`, etc.

This problem is solved by the `useEffect()` hook, which expresses a combination of `componentDidMount()`, `componentDidUpdate()`, and `componentDidUnmount()`, thereby removing redundant logic.

## **Code reusability**

Earlier, in order to organize components through lifecycle methods, we were forced to write the same code with the same logic in different components. Thus, beating the [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)(do not repeat yourself) principle.

However, with react hooks, we can now extract stateful logic so that it can be reused in other components.

# **Conclusion**

Introducing hooks in React has made it quite easier for beginners to learn and understand how the entire state of the application is managed. Hooks allow developers to write cleaner and more organized code without having to write the same code in several places, i.e., hooks enable [code reusability](https://cloudemployee.co.uk/blog/code/the-importance-of-code-reusability-in-software-development).

## References:

- [HacktoberFest 2022](https://hacktoberfest.com/)
- [HacktoberFest with Aviyel](https://aviyel.com/post/3738/announcing-hacktoberfest-with-aviyel)
- [Hacksquad](https://www.hacksquad.dev/)
- [React Documentation](https://reactjs.org/docs/hooks-intro.html)
