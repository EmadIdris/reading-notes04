# Readings: Node Ecosystem, TDD, CI/CD

## ```Array.prototype.map()```

> The ```map()``` method creates a new array populated with the results of calling a provided function on every element in the calling array.

```
const array1 = [1, 4, 9, 16];

// pass a function to map
const map1 = array1.map(x => x * 2);

console.log(map1);
// expected output: Array [2, 8, 18, 32]
```

### Syntax

```
// Arrow function
map((element) => { ... })
map((element, index) => { ... })
map((element, index, array) => { ... })

// Callback function
map(callbackFn)
map(callbackFn, thisArg)

// Inline callback function
map(function callbackFn(element) { ... })
map(function callbackFn(element, index) { ... })
map(function callbackFn(element, index, array){ ... })
map(function callbackFn(element, index, array) { ... }, thisArg)
```
## Description

> map calls a provided callbackFn function once for each element in an array, in order, and constructs a new array from the results. callbackFn is invoked only for indexes of the array which have assigned values (including undefined).

It is not called for missing elements of the array; that is:

+ indexes that have never been set;
+ indexes which have been deleted.

#### When not to use map()

> Since map builds a new array, using it when you aren't using the returned array is an anti-pattern; use forEach or for...of instead.

You shouldn't be using map if:

you're not using the array it returns; and/or
you're not returning a value from the callback.
Parameters in Detail
callbackFn is invoked with three arguments: the value of the element, the index of the element, and the array object being mapped.

> If a thisArg parameter is provided, it will be used as callback's this value. Otherwise, the value undefined will be used as its this value. The this value ultimately observable by callbackFn is determined according to the usual rules for determining the this seen by a function.

map does not mutate the array on which it is called (although callbackFn, if invoked, may do so).

> The range of elements processed by map is set before the first invocation of callbackFn. Elements which are assigned to indexes already visited, or to indexes outside the range, will not be visited by callbackFn. If existing elements of the array are changed after the call to map, their value will be the value at the time callbackFn visits them. Elements that are deleted after the call to map begins and before being visited are not visited.

Warning: Concurrent modification of the kind described in the previous paragraph frequently leads to hard-to-understand code and is generally to be avoided (except in special cases).

Due to the algorithm defined in the specification, if the array which map was called upon is sparse, resulting array will also be sparse keeping same indices blank.

### ```What is Array.reduce() in JavaScript?```

> The reduce() method executes a user-supplied “reducer” callback function on each element of the array, passing in the return value from the calculation on the preceding element. The final result of running the reducer across all elements of the array is a single value.

+ Perhaps the easiest-to-understand case for reduce() is to return the sum of all the elements in an array.

> The reducer walks through the array element-by-element, at each step adding the current array value to the result from the previous step (this result is the running sum of all the previous steps) — until there are no more elements to add.

### Syntax

```
// Arrow function
reduce((previousValue, currentValue) => { ... } )
reduce((previousValue, currentValue, currentIndex) => { ... } )
reduce((previousValue, currentValue, currentIndex, array) => { ... } )
reduce((previousValue, currentValue, currentIndex, array) => { ... }, initialValue)

// Callback function
reduce(callbackFn)
reduce(callbackFn, initialValue)

// Inline callback function
reduce(function(previousValue, currentValue) { ... })
reduce(function(previousValue, currentValue, currentIndex) { ... })
reduce(function(previousValue, currentValue, currentIndex, array) { ... })
reduce(function(previousValue, currentValue, currentIndex, array) { ... }, initialValue)
```

## Description

> The ECMAScript spec describes the behavior of reduce() as follows:

> callbackfn should be a function that takes four arguments. reduce calls the callback, as a function, once for each element after the first element present in the array, in ascending order.

> callbackfn is called with four arguments:

+ the previousValue (value from the previous call to callbackfn)
+ the currentValue (value of the current element)
+ the currentIndex, and
+ the object being traversed

> The first time that callback is called, the previousValue and currentValue can be one of two values:

+ If an initialValue was supplied in the call to reduce, then previousValue will be equal to initialValue and currentValue will be equal to the first value in the array.
+ If no initialValue was supplied, then previousValue will be equal to the first value in the array and currentValue will be equal to the second.
It is a TypeError if the array contains no elements and initialValue is not provided.

reduce does not directly mutate the object on which it is called but the object may be mutated by the calls to callbackfn.

> The range of elements processed by reduce is set before the first call to callbackfn. Elements that are appended to the array after the call to reduce begins will not be visited by callbackfn. If existing elements of the array are changed, their value as passed to callbackfn will be the value at the time reduce visits them; elements that are deleted after the call to reduce begins and before being visited are not visited.

+ If the array only has one element (regardless of position) and no initialValue is provided, or if initialValue is provided but the array is empty, the solo value will be returned without calling callbackFn.

+ If initialValue is provided and the array is not empty, then the reduce method will always invoke the callback function starting at index 0.

*** 

**Provide code snippets (in Portuguese, using a Portuguese API) showing how to use superagent() to fetch data from a URL and log the result**

> **With normal Promise .then() syntax**  
```js
'use strict';

const superagent = require('superagent');

let expectedFood = 'Banana, da terra, crua'; // Você fala português, certo?

let promiseBanana = superagent('GET', 'https://taco-food-api.herokuapp.com/api/v1/food/175')
  .then(function onResult(res) {
    (expectedFood === res.body[0].description)
    ? console.log('Banana Tempo!', res.body) // It worked... Party time.
    : console.log('Desculpe amigo... Sem fatos de banana aqui! :( '); // This is not the banana you're looking for.
  });
```

> **Again with async / await syntax**  
```js
'use strict';

const superagent = require('superagent');

let expectedFood = 'Banana, da terra, crua'; // Você fala português, certo?

async function promiseBanana(expectedFood) {
  let res = await superagent('GET', 'https://taco-food-api.herokuapp.com/api/v1/food/175');
  (expectedFood === res.body[0].description)
  ? console.log('Banana Tempo!', res.body) // It worked... Party time.
  : console.log('Desculpe amigo... Sem fatos de banana aqui! :( '); // This is not the banana you're looking for.
};

promiseBanana(expectedFood);
```

**Explain promises as though you were mentoring a Code 301 level student:**

Promises are JavaScript objects that link two things:
1. Code that may take some unknown amount of time to get information
2. Code that needs that information to continue

**Are all callback functions considered to be Asynchronous? Why or Why Not?**

No. Functions need to be told to be run async or they will be run synchronously. Usually things that rely on unreliable timing (getting data, reading a file, etc.) and would keep your program from running should be be run asynchronously. 
