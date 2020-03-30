# 13. Maintain self-resetting state in your observable streams using the scan operator

#### [📹 Video](https://egghead.io/lessons/rxjs-maintain-self-resetting-state-in-your-observable-streams-using-the-scan-operator)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson-13/src/lesson-code/TaskProgressService.js)

## Summary

- Our manager, unaware of how much our functional reactive approach has kept us delivering these features on time and bug-free, decides they **want a small new feature added to the spinner before the next release:** **a percentage indicator**, showing how many tasks have finished out of the total started since the spinner was last shown.
- So in this lesson we will be looking at **combining the existing observables that gives the up to date count of tasks**, together with a more advanced use of the scan operator, to create a stream that tells us the total count of tasks that have been launched since the spinner was last shown, and how many of them have completed.
- We’ll also take advantage of scan’s disposal behavior to reset its state when the spinner hides.
