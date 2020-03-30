# 12. Use combineLatest to only emit notifications when certain events have happened

#### [📹 Video](https://egghead.io/lessons/rxjs-use-combinelatest-to-only-emit-notifications-when-certain-events-have-happened)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson-12/src/lesson-code/TaskProgressService.js)

## Summary

- Having just congratulated us on the very quick and bug-free turn-around of our previous work item, our manager pings us again to tell us that this time, some tasks finish very shortly after our 2 second threshold.
- So **users are still seeing the glitchy spinner behavior.** Our new requirement is that once we start showing the spinner, we need to show it for at least 2 seconds, even if there are no more tasks in the background.
- **To solve this, we will create another proxy,** this time for the hiding set of events, and use the combineLatest to wait for two events to happen before we can hide the spinner: **we actually get the instruction to hide it (no more tasks in the background) and at least 2 seconds have passed.**

## Transcript
