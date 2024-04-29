#### Class Component Lifecycle

- First method is called `componentDidMount()` React will call this method when the component was just mounted.So when it was evaluated and now rendered to the DOM. It is basically the equivalent to using useEffect with an empty dependency array. `useEffect(..., [])`

- `componentDidUpdate()` Once the component was updated, when state is changed. It is basically the equivalent to using useEffect with a dependency array. `useEffect(..., [someValue])`

- `componentWillUnmount()` Called right before the component is unmounted. right before removed from DOM. It is basically the equivalent to is the cleanup function. This cleanup function is excutes right before the effect function is executed again and also again, when the component is about to removed from the DOM

`useEffect(()=> {
return () => {
...
}
},[])`
