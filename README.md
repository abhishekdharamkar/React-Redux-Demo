REACT REDUX

its use to state management

earliar we use props for sending data but its unidirectional  (top to bottom)

Redux Store use to store a data so later we use that data in any component 

Redux Basic:-
Action,Reducer,State,store

Action:- pure Object 
Action Creater:- function  e.g function for increment decrement

Reducer :- Reducer Function Can take current state and An Action as argument and return a new state

Store:- The redux store bring state,action and reducer that make up your app
you have onlly single store in a redux apps

Every Redux store has single root reducer function

redux is responsible to  to combined multiple reducer  

UseSelectors :- its use to retrive  state  from store 

Ui -----------> ACTIONS------------> REDUCERS ---------------------> STORE ---------->Ui
dispatch()      type:"ADD"	         action.type                     store={store}    update state
add(data)       payload:number       action.payload				                      useSelector()
                                     (update state) 

npm i react-redux
npm i redux

--------------------------------------
React Thunk

npm i redux-thunk
                                                                                
By default, Redux’s actions are dispatched synchronously, which is a problem for any non-trivial(having some variables or terms that are not equal to zero or an identity)
app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.

There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga.
