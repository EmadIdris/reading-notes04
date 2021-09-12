# Readings: State and Props

## React: Component Lifecycle Events

![](https://miro.medium.com/max/2000/0*pqn5ljaOw4kWrUdF)

> React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

![](https://miro.medium.com/max/2000/0*0saPKFiTUk6W3FYp)

+ ## Mounting

> When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

+ ## Updating

> Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.

+ ## Unmounting

> The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.

***

```
class FishTableRow extends React.Component {
constructor() {
super(props); //gives us access to props
//Don’t call this.setState() here
this.state = { //intitialize local state
showDescription: false
}; }
```

## ``` render() ``` 

> Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders. I also should not directly interact with the browser. render will not be invoked if shouldComponentUpdate() returns false. Here is an example of using render.


```
ReactDOM.render(
<FishTable fishes= {fishData}/>,//set fishes document.getElementById(‘app’)
);
```

***

## ``` componentDidMount() ``` 

> This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().

```
componentDidMount() {
console.log(‘got videos’);
this.getVideos(‘cats’);
}
getVideos(query) {
var options = {
key: this.props.YOUTUBE_API_KEY,
query: query
};
```

![](https://miro.medium.com/max/778/1*4y9V5936WdJKaIeVPFEa3w.png)

***

## ``` componentWillUnmount() ``` 

This method allows you to clean up the DOM and netwrok requests/ subscriptions.


***
***

## React Bootstrap

### Why React-Bootstrap?

> React-Bootstrap is a complete re-implementation of the Bootstrap components using React. It has no dependency on either bootstrap.js or jQuery. If you have React setup and React-Bootstrap installed, you have everything you need.
Methods and events using jQuery is done imperatively by directly manipulating the DOM. In contrast, React uses updates to the state to update the virtual DOM. In this way, React-Bootstrap provides a more reliable solution by incorporating Bootstrap functionality into React's virtual DOM. Below are a few examples of how React-Bootstrap components differ from Bootstrap.

***

### A Simple React Component

The CSS and details of Bootstrap components are rather opinionated and lengthy. React-Bootstrap simplifies this by condensing the original Bootstrap into React-styled components.

```
import * as React from 'react';

function Example()  {
  return (
    <div class="alert alert-danger alert-dismissible fade show" role="alert">
      <strong>Oh snap! You got an error!</strong> 
      <p> 
        Change this and that and try again.
      </p>
      <button type="button" class="close" data-dismiss="alert" aria-label="Close">
        <span aria-hidden="true">&times;</span>
      </button>
    </div>
  )
}
```

**React-Bootstrap**

```
import * as React from 'react';
import Alert from 'react-bootstrap/Alert';

function Example() {
  return (
    <Alert dismissible variant="danger">
      <Alert.Heading>Oh snap! You got an error!</Alert.Heading>
      <p>
        Change this and that and try again.
      </p>
    </Alert>
  )
}
```

```
function AlertDismissible() {
  const [show, setShow] = useState(true);

  return (
    <>
      <Alert show={show} variant="success">
        <Alert.Heading>How's it going?!</Alert.Heading>
        <p>
          Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget
          lacinia odio sem nec elit. Cras mattis consectetur purus sit amet
          fermentum.
        </p>
        <hr />
        <div className="d-flex justify-content-end">
          <Button onClick={() => setShow(false)} variant="outline-success">
            Close me y'all!
          </Button>
        </div>
      </Alert>

      {!show && <Button onClick={() => setShow(true)}>Show Alert</Button>}
    </>
  );
}

render(<AlertDismissible />);
```


