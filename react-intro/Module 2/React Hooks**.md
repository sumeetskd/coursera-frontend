## Self Notes:

Hooks: introduced in react 16.8
Functions that let you hook into react state and lifecycle feature from components.

It is used to manage state within a component and keep track of it. To use useState, you need to import it from React and then declare a state variable using array destructuring. The first element of the array is the state variable, and the second element is the function to update the state.

eg: useState Hook : can be used to track any type of data, boolean, numbers etc


import React, {useState} from 'react';

Declare a state variable:

const [state, setState] = useState(initialState);

//we use array-destructuring to store the data
-> we can use any name for the state variable
const [showMenu,setShowMenu] = useState();

Without Array Destructuring: it will be a long process

var menuState = useState(false);
var showMenu = menuState[0];	//access first item in array
var setShowMenu = menuState[1];//access second item in array

Simplied using destructure:

const [showMenu,setShowMenu] = useState(false);

useState is doing two thing:
1. Creates a state variable with an initial value -> false ->showMenu
2. Creates a function to set that state variable's value -> setShowMenu

use setShowMenu to update the showMenu -> setShowMenu(true);

-> use case: 
Hooks can be called only at the top level and only from React functions.

```
....
const [showMenu,setShowMenu] = useState(false);
//Here useState is used to track the boolean type of data
it can be used to track string, number, arrays, boolean, or object

return(
<div>
	<Child1 />
	<Child2 />
	<Child3 />
</div>
);
....
```

## Imp Points from Course

Sure! Here are the important points from the given text:

1. Introduction to Hooks: React hooks were introduced in React version 16.8 and are functions that allow you to hook into React state and lifecycle features from components.

2. useState Hook: One of the most commonly used hooks is useState. It is used to manage state within a component and keep track of it. To use useState, you need to import it from React and then declare a state variable using array destructuring. The first element of the array is the state variable, and the second element is the function to update the state.

3. Initializing State: When using useState, you can provide an initial value for the state variable. In the example given, the state variable showMenu is initialized with a value of false.

4. Updating State: The setState function, in this case, setShowMenu, is used to update the value of the state variable. By passing a new value to setShowMenu, the state variable showMenu is updated accordingly.

5. Tracking Different Data Types: useState can be used to track various types of data, including strings, numbers, arrays, Booleans, or objects. It allows you to track any data relevant to your component and use case.

6. Building Custom Hooks: In addition to the built-in hooks like useState, developers can create their own custom hooks to extract reusable component logic into separate functions. This enables better code organization and reusability.

7. Benefits of Hooks: Hooks simplify and improve the readability of React code. They offer a more organized and streamlined way to manage state and logic within components.

8. Call at Top Level: The useState hook should always be called at the top level of your component, not inside nested functions or conditionals.

In summary, the video introduces React hooks and focuses on the useState hook, which is used to manage state within a component. It explains how to initialize state, update state, and the benefits of using hooks in React applications. Additionally, developers can create custom hooks to extract and reuse component logic.
