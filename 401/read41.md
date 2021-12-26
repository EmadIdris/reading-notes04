# Compare and Contrast Redux Toolkit with Redux “Ducks”
These three concepts are probably the ones most commonly referred to in complaints about "boilerplate". I was going to cover each of these separately and in detail, but then I realized that there's already a well-written document that addresses why these concepts exist and why they're a good thing: the "Reducing Boilerplate" page in the Redux docs.

I'll quickly summarize the main points:

    Actions: Describing updates as plain serializable action objects enables time-travel debugging and hot reloading
    Action constants: Help with consistent naming conventions, make it easier to see what action types are used in an application, help prevent typos, and allow static analysis of code in IDEs
    Action creators: Encapsulate logic around creating actions, reduce duplication, allow moving logic out of components, and act as an API.

# What is the principle advantage of Redux Toolkit
![](https://cdn2.hubspot.net/hubfs/7088297/GenUI_April_2020/Images/modular-redux-tutorial-redux-toolkit.png)
**Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code. Redux Toolkit is beneficial to all Redux users regardless of skill level or experience.**


***

### Summary

- [getting started with react native](https://reactnative.dev/docs/getting-started)
- [react native basics (Tutorial)](https://reactnative.dev/docs/tutorial)
- [react native](https://reactnative.dev/)
- [expo](https://expo.dev/)
  - Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.
- [expo snack](https://snack.expo.dev/)
  - Expo Snack is an open-source platform for running React Native apps in the browser.
- [ejecting](https://docs.expo.dev/expokit/eject/?redirected)
  - If you created an Expo project and you want a way to add custom native modules, this guide will explain how to use ExpoKit for that purpose.
    Normally, Expo apps are written in pure JS and never "drop down" to the native iOS or Android layer. This is core to the Expo philosophy and it's part of what makes Expo fast and powerful to use.
    However, there are some cases where advanced developers need native capabilities outside of what Expo offers out-of-the-box. The most common situation is when a project requires a specific Native Module which is not supported by React Native Core or the Expo SDK.
    In this case, Expo allows you to eject your pure-JS project from the Expo iOS/Android clients, providing you with native projects that can be opened and built with Xcode and Android Studio. Those projects will have dependencies on ExpoKit, so everything you already built will keep working as it did before.
    We call this "ejecting" because you still depend on the Expo SDK, but your project no longer lives inside Expo Go. You control the native projects, including configuring and building them yourself.

***

| Term       |       Definition             |
| -----------|------------------------------|
|redux toolkit slices|A function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. This API is the standard approach for writing Redux logic|
|namespace|he use of Namespace makes the JavaScript code modular and structured also easy to read, understand and modify. So without polluting the global namespace, we can achieve all these things, any way we have to use the global namespace but we are not messing things there.|

