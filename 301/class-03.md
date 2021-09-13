# Readings: Passing Functions as Props

## Lists and Keys

![](https://i.ytimg.com/vi/0sasRxl35_8/maxresdefault.jpg)

## 1.

```
const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);
```

This code logs  to the console

```
 [2, 4, 6, 8, 10] .

```
***

## 2.
```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);

ReactDOM.render(
  <ul>{listItems}</ul>,
  document.getElementById('root')
);
```

***

## 3. 

## Each list item needs a unique **key**.

***

## 4.

**Keys** are used by **React** to ***identify changed, added or remobed items***.

***
***

## The Spread Operator

![](https://i.morioh.com/2019/11/19/580be7d831c1.jpg)

![](https://image.slidesharecdn.com/areactjourney-160630135059/95/a-react-journey-16-638.jpg?cb=1467294736)


## 1. 

 > It's an operator that is used for adding items to arrays, combining arrays or objects, and spreading an array out into a function's arguments.

![](https://i.stack.imgur.com/wuV5l.png)

***

## 2. 

- Copying an array.

- Combining arrays.

- Using an array as a function.

- Adding an item to a list.

***
## 3.

```
const array1 = ['a',`ab`,`abc`]
const array2 = [`d`,`de`,`def`]
const arrayconcat = [...array1,...array2]
console.log(...arrayconcat) 
```
***

## 4.

```
const names = ['nathan', 'ahmad', 'john'];
const moreNames = ['mike', ...names];
console.log(moreNames);
```
***

## 5.

```
const objectOne = {p1: 'Hello Im object 1'};
const objectTwo = {p2: 'Hellow Im object 2'};
const objectThree = {...objectOne, ...objectTwo, p3: 'Hellow Im object 3'};
console.log(objectThree);
const objectFour = {...objectOne, ...objectTwo, p4: () => {console.log("Hellow Im object 4".repeat(5))}};
objectFour.p4();
```

## Passing Functions Between Components


### 1. 

> He used the **map() function** to loop over the array of objects.
He loop through the array that need to be modified by using the map method with the access to that array with this.state.people (the name of the array),Then he return the created object that will access to each object inside the array so it will be modified.


***

### 2. 

> This function **loops over the array of objects** to **find the passed name** to be able to update/increment the count*
It will loop inside the objectof the main array and find a matching with the data that has been passed to the function, then it will increament the count inside the object that has been passed.Then it returned to the new variable that been declared, so after that it update the state of the object in the main array.
***

### 3. 

> In order to **pass a method** from a **parent** to a **child** you basically need to use **props** , In the child component at itâ€™s own function we pass it with this.props with the name of the function weâ€™ve create it to change the state in the parent component as calling it with the data that we need to change.

***

### 4. 

> and in the parent component we pass it as any other props by name and the value that refrence to the funtion we created to change the state of the objects. When the action that we need to been taken from the user is done,like in the vidoe click on the button, the method we called that we added to the child componant function which will be sended to the parent componant and make the state changed.
