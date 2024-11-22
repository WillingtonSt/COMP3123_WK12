## Redux Store Configuration (`./app/store.js`)

The Redux store is created using `configureStore` from Redux Toolkit. This function simplifies store setup and accepts a configuration object. 

- **`reducer` key:** Maps the state slice `counter` to the `counterReducer` function. This ensures that the state managed by `counterReducer` is stored under the `counter` key in the global Redux state.

---

## Counter Slice (`./features/counter/counterSlice.js`)

The `counterSlice` manages the state and logic for a "counter" feature



## Counter Component (`./features/counter/Counter.js`)

The `Counter` component is a React component that displays and updates a counter value using Redux. It retrieves the current counter value from the Redux store using `useSelector` and updates the value by dispatching actions (`increment`, `decrement`, and `incrementByAmount`) using `useDispatch`. 

Users can:
- Increment or decrement the counter by 1 using buttons.
- Increment the counter by a specific amount entered in an input field.

This setup demonstrates state management with Redux Toolkit in a simple React app.