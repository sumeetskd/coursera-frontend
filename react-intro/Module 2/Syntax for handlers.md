## Self Notes:

event 	   -> 	event Handler -> Action
(click)		(onClick)	(Open Menu)

HTML Event Handling:

```
<button id = "js-btn"
onclick = "clickHandler()"> Click me! </button>
```
React Equivalent of above code:
```
<button
onClick={clickHandler}>
Click me!</button>
```
onclick is converted to camelcase, ie. onClick
and delemiter-expression {} is used to make the function call to clickHandler() function

React is passing these function Declations as Props:

App Component:
```
return (
	<Counter onClick={clickHandler}/>
)
```

Read me:

Sure! Here are the important points from the given text:

1. Events in Browsers: Interactions like clicking buttons, scrolling, or canceling notifications produce events in the browser.

2. Event Handlers: Event handlers are used to execute actions in response to events. For example, a button click can trigger an event handler that opens a menu.

3. HTML Event Handling: In plain HTML, event handlers are added using attributes like `onclick` with the name of the corresponding function to execute.

4. JavaScript Approach: Using JavaScript, event handling involves two steps: accessing the HTML element using JavaScript and then attaching an event listener using `addEventListener`.

5. React's Declarative Approach: React prefers a declarative approach, avoiding direct manipulation of the DOM. Event handling is done using event attributes in JSX.

6. React's JSX Event Handling Syntax: The event attributes in React JSX start with "on" and have the event name with the first letter capitalized. The function reference is passed without invocation within curly braces.

7. Function Declarations as Props: React allows passing function declarations as props between components. For example, passing an `onClick` prop from a parent component to a child component.

In summary, the video explains the syntax differences between event handling in plain HTML and React. It emphasizes the declarative nature of React and how event handling is done using JSX attributes and function references without invoking them directly. Additionally, it mentions passing function declarations as props between components in React.
