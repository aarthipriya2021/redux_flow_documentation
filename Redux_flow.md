<h1 align="center">Redux<h1>
<h4> Redux is a predictable state container of JS apps. In large applications, there is a need to store the state at a central location and share it among the different components. <h4>
  
> State management system for cross component
<p align="center">
  <img src="https://reactjsexample.com/content/images/2021/11/Redux-Concepts-and-data-flow.jpg" width="350" title="Redux flowt">
</p>

- Redux uses one way data flow app structure.
- State describes the condition for the app at a point in time and UI renders based on the state.
- When somethings happen in the app
    -  The UI dispatches an action.
    -  The store runs the reducers, and the state is updated based on what they occurred.
    -  The store notifies the the UI that the state has changed.
<h3>Core Principle</h3> <br />
1. States of whole application is stored in single store.
2. The only way to change the state is to emit an action , an object describing what happened.
3  To specify how the state transformed by an action, write pure function.
  
