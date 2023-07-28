Title: Efficient State Management with Context API, useContext, and useReducer

**Introduction**
- As React apps grow complex, efficient state management becomes crucial.
- Passing states via props can be cumbersome for deeply nested components.
- Context API offers a more efficient way to manage state across components.

**Context API: A Teleportation Approach**
- Context API eliminates the need for prop drilling by creating a centralized state store.
- Set up a context provider to hold the state and provide it to components.
- Components can be context consumers and access the state directly without intermediaries.

**Example App**
- Illustrates a simple app for monitoring daily meal plan and food intake.
- Components: App, mealsList, counter.

**Meals Provider: Setting Up Context**
- The meals provider is a context provider that stores the state (today's meals array).
- Use `React.createContext()` to create the context variable (`mealsContext`).
- `mealsProvider` component wraps children with `mealsContext.Provider` and provides the state (`meals`).
- Use `useContext()` to access the context data in mealsList and counter components.

**Meals List Component**
- Destructure `meals` from the context data received via `useContext()`.
- `meals` holds an array of food items.
- Map over `meals` to render an H2 element for each item.

**Counter Component**
- Similar to meals list, access context data (`meals`) using `useContext()`.
- No need for prop drilling; components directly access the state via the context.

**Introduction to useReducer Hook**
- `useReducer` is a superpower for state management.
- It takes an initial state and a reducer function.
- Instead of `setState`, use `dispatch` method with an object containing an action type.

**Example of useReducer**
- Illustrates a rideshare app with wallet money state.
- The initial state is 100, and actions are "Pick Up Customer" (increase) and "Refuel Vehicle" (decrease).
- The reducer function handles state changes based on action type.

**Conclusion**
- Context API and hooks like `useContext` and `useReducer` enhance state management in React apps.
- These tools allow more efficient handling of state across multiple levels of components, reducing complexity and redundancy in the code.
