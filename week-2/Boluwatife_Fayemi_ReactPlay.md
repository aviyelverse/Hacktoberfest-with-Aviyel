# **Introduction**

[[React](https://reactjs.org/)](https://reactjs.org/) is a [[javascript](https://www.javascript.com/)](https://www.javascript.com/) framework that makes building [[user interfaces (UI)](https://www.techtarget.com/searchapparchitecture/definition/user-interface-UI)](https://www.techtarget.com/searchapparchitecture/definition/user-interface-UI) easy. React apps are usually made of components coupled together to build user interfaces(UI). User interfaces present data and offer interaction to users. These components simplify the process of building complex user interfaces. They help programmers avoid repetition and also give room for reusability.

In this guide, you will learn about the following:

- **React props**
- **React state**
- **How and why do we use react props and states?**
- **The distinction between react props and state**

# What are props?

Props are short for properties. Props are used to pass data into a component. It works the same way parameters work for functions.

## Why Do We Really Need or Make Use of Props?

As earlier mentioned, components are the fundamental building blocks of React apps. These components are usually used to define the structures of user interfaces and render data. More often than not, there are cases where the structures of React components are the same but the data to be presented by each of them is different.

In the above-mentioned scenario, should several components be created and modified to the data within each component despite the bolded? As you have thought, this is not an elegant solution, as doing this goes against the DRY (Don’t Repeat Yourself) principle. This is where props come in handy. In order to fully understand what props are, let’s relate them to what we are already familiar with-HTML Attributes.

## Using the input element in HTML as an example

The HTML input element comes in various types. The type one intends to use can be determined by passing in the type as the value for the type attribute. What does that mean? It implies that the attribute controls the type of input rendered on a page. To explain more, I could display a calendar or password input by just changing the attribute value for type while still using the same input element. What has changed? Only the attribute value has changed. Props work the same way in React as well.

Back to React: enough with the HTML analogy!

Let’s use [[Reactplay's](https://reactplay.io/)](https://reactplay.io/) website homepage as a case study. See the image below.

![image](https://user-images.githubusercontent.com/67077455/204149665-197a8d4f-890e-4c46-ac06-87b9a713074e.png)
You should notice that the highlighted parts look identical in terms of structure even though the data presented is different.  Each of them has an image, title, author’s image, author name, like button, like count, and programming language logo. These highlighted parts are components. But how are they able to render different data? The data to be displayed by a component is passed in as props. So different data could be passed as the value of a prop to the same component. This makes components flexible and dynamic.

![image](https://user-images.githubusercontent.com/67077455/204149703-5acd5368-98cf-4784-a162-9e180c9226a7.png)

In summary, props are used to render dynamic content.

Passing props is how information flows in React apps, from parents to children.

## Using Props in a Component

Props are passed in components just like HTML attributes. Props are accessed or received within a functional component as a function parameter, usually named props. Props received in a component are javascript objects, and their property values can be accessed using javascript dot notation.

# What is State?

“State refers to the value that is managed by a component similar to variables declared inside a function. Anytime you have to change values that should be saved or displayed, you’ll likely be using a state.” State is used to remember things within a component.

## Why Do We Really Need or Make Use of State?

Over the years, the user interface has evolved from just rendering or displaying data on the browser page. There is a need for more interaction. Users need to click buttons, move the cursor and see changes on the page as they perform these events.

Updating the state will cause DOM re-rendering which makes the UI interactive.

## Using State in a Component

State usually starts off with a default value the first time a component renders on the DOM.

The state is managed within a component. The value for the state can be updated using the setState() function. Whenever the value for state changes, React automatically handles re-rendering the components.

# Differences between Props and the State

Props and state are core concepts in React. Therefore, it is very important to understand the difference between them.

Having discussed their concepts and why to use them above, this section gives you an insight into the differences between them

The differences between props and state are summarized in the table below.

![image](https://user-images.githubusercontent.com/67077455/204149740-df92ffdc-c3c5-4306-b6f1-6a9ce2615c47.png)

## Conclusion

While Props and state are two different concepts in some ways in React, they are usually used together to build functional react applications.

If you are interested in trying out and learning more about the concepts illustrated in this guide, you could head over to ReactPlay, an open-source platform that helps you learn, create and share ReactJS projects with the developer community.

# Additional Resources

[[React-guide on state vs. props](https://github.com/uberVU/react-guide/blob/master/props-vs-state.md)](https://github.com/uberVU/react-guide/blob/master/props-vs-state.md)

What is the difference between state and props in react? on [Stackoverflow](https://stackoverflow.com/questions/27991366/what-is-the-difference-between-state-and-props-in-react#:~:text=props%20are%20passed%20via%20component,the%20UI%20when%20values%20changes.)

React Docs on [[State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)](https://reactjs.org/docs/state-and-lifecycle.html)
