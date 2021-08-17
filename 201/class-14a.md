# Readings

## Transforms
> With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.
The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

## Transform Syntax

> The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```
## 2D Transforms
Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane.

+ 2D Rotate
> The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees.

```
<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>

***

.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}

```
+ 2D Scale

> Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

```
<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>

.box-1 {
  transform: scale(.75);
}
.box-2 {
  transform: scale(1.25);
}

```

+ 2D Translate

> The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

```
<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>
<figure class="box-3">Box 3</figure>

.box-1 {
  transform: translateX(-10px);
}
.box-2 {
  transform: translateY(25%);
}
.box-3 {
  transform: translate(-10px, 25%);
}

```

+ 2D Skew

The distance calculation of the skew value is measured in units of degrees. Length measurements, such as pixels or percentages, do not apply here.

```
<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>
<figure class="box-3">Box 3</figure>

.box-1 {
  transform: skewX(5deg);
}
.box-2 {
  transform: skewY(-20deg);
}
.box-3 {
  transform: skew(5deg, -20deg);
}
```

## Transitions & Animations

One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

### Transitions

> As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

```
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```
#### Vendor Prefixes

```
.box {
    background: #2db34a;
    -webkit-transition-property: background;
       -moz-transition-property: background;
         -o-transition-property: background;
            transition-property: background;
    -webkit-transition-duration: 1s;
       -moz-transition-duration: 1s;
         -o-transition-duration: 1s;
            transition-duration: 1s;
    -webkit-transition-timing-function: linear;
       -moz-transition-timing-function: linear;
         -o-transition-timing-function: linear;
            transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```

### Transition Timing

> The linear keyword value identifies a transition moving in a constant speed from one state to another. The ease-in value identifies a transition that starts slowly and speeds up throughout the transition, while the ease-out value identifies a transition that starts quickly and slows down throughout the transition. The ease-in-out value identifies a transition that starts slowly, speeds up in the middle, then slows down again before ending.

```
.box {
  background: #2db34a;
  border-radius: 6px;
  transition-property: background, border-radius;
  transition-duration: .2s, 1s;
  transition-timing-function: linear, ease-in;
}
.box:hover {
  background: #ff7b29;
  border-radius: 50%;
}
```

```
.box {
  background: #2db34a;
  border-radius: 6px
  transition-property: background, border-radius;
  transition-duration: .2s, 1s;
  transition-timing-function: linear, ease-in;
  transition-delay: 0s, 1s;
}
.box:hover {
  background: #ff7b29;
  border-radius: 50%;
}
```

### Transitional Button

```
<button>Awesome Button</button>

button {
  border: 0;
  background: #0087cc;
  border-radius: 4px;
  box-shadow: 0 5px 0 #006599;
  color: #fff;
  cursor: pointer;
  font: inherit;
  margin: 0;
  outline: 0;
  padding: 12px 20px;
  transition: all .1s linear;
}
button:active {
  box-shadow: 0 2px 0 #006599;
  transform: translateY(3px);
}
```
### Animations

> To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

```
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
```
### Animation Duration, Timing Function, & Delay

> Once you have declared the animation-name property on an element, animations behave similarly to transitions. 

```
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
}

.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: .5s;
}

<div class="stage">
  <figure class="ball"></figure>
</div>

@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
.stage {
  height: 150px;
  position: relative;
}
.ball {
    height: 50px;
    position: absolute;
    width: 50px;
}
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: .5s;
}

```

### CodePen Home 6 Buttons animated

HTML

```
<div class="group">
		<button class="blam">Blam</button>
		<button style="-webkit-animation-delay: .3s;animation-delay: .3s;" class="syke">Syke</button>
		<button style="-webkit-animation-delay: .6s;animation-delay: .6s;" class="later">Later</button>
</div>
```
CSS

```
@import url(https://fonts.googleapis.com/css?family=Droid+Sans:700);
		*{
			margin: 0;
			padding: 0;
			box-sizing: border-box;
			transition: all .1s;
		}
		body{
		background-color: #424242;
			font-family: 'Droid Sans', sans-serif;
		}
		.group{
			text-align: center;
			margin: 20px auto;
		}
		.group button{
			margin-top: 10px;
		}
		button{
/*			box-sizing: border-box;*/
			background: NONE;
			border: none;
			outline: none;
			border-radius: 3px;
			padding: 15px 70px;
			color:white;
			text-transform: uppercase;
			font-weight: 700;
			text-shadow: 0 1px 3px rgba(0, 0, 0, 0.41);
			box-shadow: 0 3px 0 0 #383838;
			border:3px solid transparent;
			
		
			animation: pulse 1s linear infinite alternate;
			-webkit-animation: pulse 1s linear infinite alternate;
		}
		.active,
		button:active{
			background-image: linear-gradient(rgba(0,0,0,.1) 13%, transparent 13%,transparent);
			box-shadow: 0 1px 0 0 #383838;
			color: rgba(0, 0, 0,.45);
			text-shadow: none;
			
			
			-webkit-animation-play-state: paused; 
    	animation-play-state: paused;
		}
		button:focus,
		button:hover{
			-webkit-animation-play-state: paused; 
    	animation-play-state: paused;
		}
		
		
		.blam:focus,
		.blam:hover{
			background-color:#0097bd;
		}
		.blam{
			background-color:#00bff0;
			border-color: #00bff0;
		}
		
		.syke:focus,
		.syke:hover{
			background-color:#ad4e4e;
		}
		.syke{
			background-color:#e06464;
			border-color:#e06464;
		}
		
		.later:focus,
		.later:hover{
			background-color:#7c8b8f;
		}
		.later{
			background-color:#a8bdc2;
			border-color:#a8bdc2;
		}
		
		@-webkit-keyframes pulse {
			100% {
				transform: translateY(6.9px); 
			} 
		}

		@keyframes pulse {
			100% {
				transform: translateY(6.9px); 
			} 
		}
```

### 404 CODE

HTML

```
<h1>4</h1>
<h1>0</h1>
<h1>4</h1>
```

CSS

```
body {
  margin:0;
  font-family:sans-serif;
  color:#f25252;
  background:#f7f7f7;
}
h1 {
  font-size:11rem;
  position:absolute;
  transform:translate(-50%,-50%);
  margin:0;
}
h1:nth-of-type(1){
  animation: range 4s infinite;
}
h1:nth-of-type(2){
  left:50%;
  top:50%;
  animation: size 4s infinite;
}
h1:nth-of-type(3){
  animation: range2 4s infinite;
}
@keyframes range {
  0%  {left:42%;top:50%;font-size:11rem;}
  25% {left:50%;top:40%;font-size:4.5rem;}
  50% {left:58%;top:50%;font-size:11rem;}
  75% {left:50%;top:60%;font-size:4.5rem;}
  100%{left:42%;top:50%;font-size:11rem;}
}
@keyframes range2 {
  0%  {left:58%;top:50%;font-size:11rem;}
  25% {left:50%;top:60%;font-size:4.5rem;}
  50% {left:42%;top:50%;font-size:11rem;}
  75% {left:50%;top:40%;font-size:4.5rem;}
  100%{left:58%;top:50%;font-size:11rem;}
}
@keyframes size {
  0%  {font-size:11rem;}
  25% {font-size:26rem;}
  50% {font-size:11rem;}
  75% {font-size:26rem;}
  100%{font-size:11rem;}
}
```




