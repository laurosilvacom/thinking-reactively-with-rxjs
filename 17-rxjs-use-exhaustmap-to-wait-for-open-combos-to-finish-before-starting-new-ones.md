# 17. Use exhaustMap to wait for open combos to finish before starting new ones

#### [📹 Video](https://egghead.io/lessons/rxjs-use-exhaustmap-to-wait-for-open-combos-to-finish-before-starting-new-ones)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson-15/src/lesson-code/TaskProgressService.js)

## Summary

- In this lesson, **we'll be looking at an issue with our combo implementation**: given that we're `switchMapping` to a new inner combo each time the user presses the combo initiation key (the letter "a" in our example), if the initiation key is found anywhere in the middle of the combo, it will just cancel out any on-going inner combos.
- To fix it, we'll look at the differences between `switchMap` and `exhaustMap`and why `exhaustMap` is a much better choice for our scenario: `switchMap` disposes of any previous inner observables when it gets a new notification from the source, while `exhaustMap` waits for the inner observable to finish, before considering any new notifications from the source.

## Transcript
