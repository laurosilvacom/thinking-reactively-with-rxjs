# 10. Encapsulate complex imperative logic in a simple observable

#### [📹 Video](https://egghead.io/lessons/rxjs-encapsulate-complex-imperative-logic-in-a-simple-observable)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson10/src/lesson-code/TaskProgressService.js)

## Summary

- **Two very important features** of the Observable primitive is that they can be **activated by subscribing to them and disposed off** when we are not interested in them anymore. All good observables **need to clean up after themselves when they are disposed off**.
- We took advantage of this when we wrote the observable that switches to showing the loader when the count is positive, and stops listening to it when the count is zero.
- In this lesson, we will learn **how to encapsulate all the complex imperative logic for showing and hiding the spinner**, inside a simple observable that can be plugged into any stream.
