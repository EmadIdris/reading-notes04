# How does React differ from vanilla JS/HTML/CSS?
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRNhFALlTwmD63noLADpbKSX20ofyoYWggW3A&usqp=CAU)

**Plain JS apps usually start with the initial UI created on the server (as HTML), whereas React apps start with a blank HTML page, and dynamically create the initial state in JavaScript. React requires you to break your UI into components, but plain JS apps can be structured in any way you see fit.**

# What is the primary difference between a function component and a class component?
![](https://miro.medium.com/max/1400/1*6-bN_FxEMfRTHZSouF8DLg.png)


| Term       |       Definition             |
| -----------|------------------------------|
|Functional Components|Functional component are much easier to read and test because they are plain JavaScript functions without state or lifecycle-hooks. You end up with less code. They help you to use best practices|
|Children / Child Components|children is a special property of React components which contains any child elements defined within the component, e.g. the divs inside Example above. {this. props. children} includes those children in the rendered result|