Basic concept:


Element want to update its state -> event dispatched -> state machine -> hook into dispatched event and return new state that the element requested

Syntax close to this:
https://recoiljs.org/docs/api-reference/core/atom

Have event-wrapper over parent element that handels the statemachine.

Have element build Objects that it sends to the statemachine to evaluate.


const counter = atom({
    key: "myCounter" // link to the state variable
    default: 0
})

const [variable, variableSetter] = litCoilState(counter) -> have method that is connected to the statemachine and can update the "atom". 