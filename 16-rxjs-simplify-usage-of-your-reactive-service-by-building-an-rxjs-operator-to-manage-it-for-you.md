# 16. Simplify usage of your reactive service by building an RxJS operator to manage it for you

#### [📹 Video](https://egghead.io/lessons/rxjs-simplify-usage-of-your-reactive-service-by-building-an-rxjs-operator-to-manage-it-for-you)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson-15/src/lesson-code/TaskProgressService.js)

## Summary

- While we’ve made sure to **expose our spinner service using simple, external APIs, most of the time, it will be called in the same way, from observables and promises**.
- In this lesson, we will be creating an RxJS operator that be easily plugged in to different observables to track them via the spinner.
