# 07. Use the filter and pairwise operators to determine when to show and hide the spinner

#### [📹 Video](https://egghead.io/lessons/rxjs-use-the-filter-and-pairwise-operators-to-determine-when-to-show-and-hide-the-spinner)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson-07/src/lesson-code/TaskProgressService.js)

## Summary

- Having access now to an observable that tells us when the in-progress task count changes, we will use it to create two even more specialized streams that will bring us close to solving our initial **problem: an event stream that fires when we need to show the spinner and another that fires when we need to hide it.**
- We will be using the pairwise and filter operators.

## Transcript
