# 11. Extend your reactive logic using observable-like proxies that delay or drop events

#### [📹 Video](https://egghead.io/lessons/rxjs-extend-your-reactive-logic-using-observable-like-proxies-that-delay-or-drop-events)

#### [💻 Code](https://github.com/rarmatei/egghead-thinking-reactively/blob/lesson-11/src/lesson-code/TaskProgressService.js)

## Summary

- **Our app is working!** But now our manager comes in and tells us that some tasks in our app are finishing very fast, so users are seeing a short glimpse of the spooner which makes the app look glitchy.
- **Our new requirement is to wait at least 2 seconds before showing the spinner.** So without introducing any complexity into our main observable, we will create a new intermediary stream that will be a proxy between the observable that immediately tells us when to show the spinner and the one that actual shows it. **This new proxy will delay the events accordingly.**

## Transcript
