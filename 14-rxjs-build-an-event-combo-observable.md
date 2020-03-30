# 14. Build an event combo observable

#### [📹 Video](https://egghead.io/lessons/rxjs-build-an-event-combo-observable)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson-14/src/lesson-code/TaskProgressService.js)

## Summary

- After another pat on the back from our manager, we get a notification that a new task has been assigned to us: _“While most users find it useful, some have asked if they can disable the spinner. Add a feature that turns off the spinner functionality once a certain combination of keys has been pressed within a time period”_.
- So in this lesson, **we will look at building an observable factory**, that can be initialized with a certain list of key codes, and will fire whenever that key combo gets pressed quickly, within a 5 second window. **We will be introducing the fromEvent, concat and takeWhile operators.**
