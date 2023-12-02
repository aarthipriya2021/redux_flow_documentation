<h1 align="center">Redux<h1>
<h4> Redux is a predictable state container of JS apps. In large applications, there is a need to store the state at a central location and share it among the different components. <h4>
  
> State management system for cross component
<p align="center">
  <img src="https://reactjsexample.com/content/images/2021/11/Redux-Concepts-and-data-flow.jpg" width="350" title="Redux flowt">
</p>

- Redux uses one way data flow app structure.
- State describes the condition for the app at a point in time and UI renders based on the state.
- When somethings happen in the app  <br />

    -  The UI dispatches an action.
    -  The store runs the reducers, and the state is updated based on what they occurred.
    -  The store notifies the the UI that the state has changed.
<h3>Core Principle</h3>  <br />

-  States of whole application is stored in single store.
-  The only way to change the state is to emit an action , an object describing what happened.
-  To specify how the state transformed by an action, write pure function.

<h2>Redux Toolkit</h2>
Redux Toolkit simplifies the process of working with redux by providing utility functions and abstractions.

<h3>Redux flow using Redux toolkit </h3>

<h4>
-  Create a slice
</h4>

In redux toolkit, you start by creating 'Slice'. A slice includes a reducer and action creators related to a specific piece of the application state.

![image](https://github.com/aarthipriya2021/redux_flow_documentation/assets/75599178/01857d2f-ec73-44c5-ac60-b5227578bdf2)

<h4>
-  Exporting action creators and reducers:
</h4>

Redux toolkit automatically generates actions creators based on the defined reducers. Export these action creators and reducer.

![image](https://github.com/aarthipriya2021/redux_flow_documentation/assets/75599178/6bfda03b-bda5-4547-b6f2-44ad1721ea80)

<h4>
-  Create Redux store
</h4>

Use the "configurestore" functions from redux toolkit for create the redux store pass in the reducer by an objects containing multiple reducers.

![image](https://github.com/aarthipriya2021/redux_flow_documentation/assets/75599178/609b9287-3a9f-4c54-97b9-cb1ad5657fd3)

<h4>
-  Dispatch Actions
</h4>

Components can dispatch actions using the action creators provided by redux toolkit. This is often done in responses to user interactions or other events. 

![image](https://github.com/aarthipriya2021/redux_flow_documentation/assets/75599178/6271f11b-8484-4699-91e6-a3cb847d1da2)

<h4>
- Access State
</h4>

Components can access the state using the 'useSelector hook provided by 'react-redux'. 

![image](https://github.com/aarthipriya2021/redux_flow_documentation/assets/75599178/271f1c3f-864a-460d-a71d-48a06e0c3e6f)

<h4>
- useDispatch() hook
</h4>

useDispatch() hook is equivalent to mapDispatchToProps function. 
This hook reference to the dispatch function from the redux store. You may use dispatch actions as you needed.

<h4>
- useSelector() hook
</h4>

useSelector() hook is equivalent to mapStateToProps function. 
It takes in a function argument that returns the part of the state that you want.

