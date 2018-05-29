Fron advanced-react-patterns courses by Kent C. Dodds

## Compound Component
- Good pattern to have parent child kind of relations
- the user should not need to have any idea of how the states are being shared
- we can handle the complex nesting of DOM using context api

- As a context.Provider `value` pass the this.state instead of new object because the new object will always have different reference even thought the values are same. So the elements under Provider will always render eventhough the values are not actually changed


## Render Props
- Simply a render function as props
- Best to separate the UI and state management 
- [Uncleared] : The test didn't passed if I user `<React.Fragment>this.props.children({on: this.state.on,toggle: this.toggle,})</React.Fragment>`. I had to unwrapp the `React.Fragment`


## State Reducer
- To let the user handle the state changes 
- changes inside the component -> notify the User -> user will make necessary changes to stage and return the updated changes -> Component should update the states as per what returned

## Control Props
- Make sure how the state should be updated. As in controlled props the state can be update the by the internal state or by the props
- We should laso take care of unncessary rerendering. So only update the internal state if necessary. Ask a que that if the rerender really necessary for the component? 
- returning null will skip the re-render

## Provider patter
- resolves the prop drilliung issue
- Create context with the data we want it to contain (i.e providers default value)
- wrap the element section under which we want to share the context using <SomeContext.Provider values={something}>
- and whereever we want to ustilize those shared values we can use <SomeContext.Consumer>



## Mistakes
- we call `this.setState(updater,callback)` , please make sure you haven't tried to create it by `this.stateState = ()=>`


  
