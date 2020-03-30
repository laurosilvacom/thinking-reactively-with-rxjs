# 05. Create safe and predictable observable abstractions

#### [📹 Video](https://egghead.io/lessons/rxjs-create-safe-and-predictable-observable-abstractions)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson-05/src/lesson-code/TaskProgressService.js)

## Summary

- Because we're thinking in terms of very isolated layers of abstractions, we're also **looking to build well abstracted observables** that make sense on their own. One way you could figure out if an observable can live on its own is: If I threw my initial requirement away, could this observable still be useful for something else?
- As part of building well designed abstractions, we need to assume they can be used in any context, and not just in the one we're focused on building at the moment. So we need to make them as predictable as possible to consumers.
- In this lesson, we'll **ensure that the stream we built previously guards against situations where we have more task completions than starts**, and also always gives an initial value.

## Transcript
