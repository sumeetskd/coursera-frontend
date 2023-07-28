## Self Notes:


Data in react can be handled by 2 methods between components:

1. Props
2. States

Props: Data comes from outside component, ie. parent component, 
-> the props data is immutable
-> the data in props belongs to the parent that renders the component

States: Data is present within the component, it uses component's data
-> it is mutable

Sure! Here are the important points from the given text:

1. Data Flow in React: React uses one-way data flow, where data moves from top to bottom through the component hierarchy. Changes are transmitted through the system, ensuring a predictable data flow.

2. Data as Props: In React, data is passed down from parent components to child components through props. Child components cannot mutate or change their props; they can only read them and re-render accordingly.

3. Data as State: React components also have state, which is data that belongs to the component itself and can be mutated. State helps manage and control data within a component.

4. Props vs. State: Props data is received from parent components and is immutable. State data is managed within the component and can be changed.

5. Example App: The example app consists of two components, App and Child. App is a class component that initializes its state with the current date. It renders the Child component with the current date passed as a prop called "message."

6. Child Component: The Child component receives the "message" prop and displays it inside an h1 element. The "message" prop is the current date converted to a string format, including the hours, minutes, and seconds.

7. Data Flow: When the app runs, the state in the App component flows down to the Child component as a prop, and the h1 element displays the current date and time.

In summary, the video explains the one-way data flow in React, where data is passed from parent to child components via props. Child components cannot mutate their props; they can only read them and re-render accordingly. Additionally, state is used to manage data within a component and can be mutated. This data flow model ensures a smooth and predictable flow of data in React applications.
