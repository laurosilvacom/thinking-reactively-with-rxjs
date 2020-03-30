# 06. Maintain shared observable state using the scan and shareReplay operators

#### [📹 Video](https://egghead.io/lessons/rxjs-maintain-shared-observable-state-using-the-scan-and-sharereplay-operators)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson-06/src/lesson-code/TaskProgressService.js)

## Summary

- The `scan()` is very useful in RxJS. It **allows you to maintain a running state over time.** In this lesson, we'll look at some of the state types scan can hold: transient or single source of truth, and how we can achieve each of them by combining it with the share operators.
- We'll also look at the differences between `share() / shareReplay(1) / shareReplay({bufferSize: 1, refCount: true})` and how to avoid memory leaks when using them.

## Transcript
