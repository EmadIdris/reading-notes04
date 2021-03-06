# Why is the Context API useful?
![](https://miro.medium.com/max/2000/1*Ha2vNB0ILaYKPXk6oyTZSQ.png)

**Context API is easy to is use as it has a short learning curve. It requires less code, and because there's no need of extra libraries, bundle sizes are reduced. Redux on the other hand requires adding more libraries to the application bundle. The syntax is complex and extensive creating unnecessary work and complexity**

# Can a component outside of a provider get its context?
**To access a React context outside of the render function, we can use the useContext hook. We create the UserContext by calling the React. createContext method with a default context value. Then in the Users component, we call the useContext hook with UserContext to accxess the current value of UserContext**

# What are some common use cases for using the Context API?
**Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context**

# Describe “Context Hell”
**Like the callback hell, usual when jQuery was used for everything, the React Context hell is the nasty code you get taking advantage of the React Context API**

| Term       |       Definition             |
| -----------|------------------------------|
|global state|Context provides a way to pass data through the component tree without having to pass props down manually at every level, managing state in multiple components that are not directly connected. ... Enough talking about it. Let me show you with some code|
|global context|The global context is the fallback context in JavaScript. ... js, that means an object with information related to Node. In the browser, the global context is the Window object. If you run a file in strict mode, then JavaScript leaves this undefined if it's not actually set.|
|provider|Custom JavaScript authentication providers are plug-in JavaScript modules that you include in JavaScript code and specify as the authentication provider for your API in API Creator. ... to run as a single node, you want to persist your authentication token|
|consumer|The Consumer component allows a React component to subscribe to the context changes. The component makes the data available using a render prop