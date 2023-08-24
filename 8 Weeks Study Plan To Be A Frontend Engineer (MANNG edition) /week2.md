The clock is ticking. I hope you have gone through the plan for week 1.

If you haven’t gone through it, go check it out before continuing Week 2.

[8 Weeks Study Plan To Be A Frontend Engineer (MANNG edition) — Week 1With hiring freeze, large-scale layoffs impacting the tech industry and a huge influx of experienced engineers on the…medium.com](https://medium.com/@FrontendJirachi/8-weeks-study-plan-to-be-a-frontend-engineer-manng-edition-week-1-758699e61e8c)

In Week 1 we brushed up on:

- JS basics
- Prototypical inheritance
- Scope
- Closure
- ES6 syntax
- array & string algorithmic questions.

**For Week — 2**

We will practice the following:

- Promise, Async request(Ajax), data fetching (fetch API)
- Date, Math API

## Promise

A Promise is **an object representing the eventual completion or failure of an asynchronous operation.** It is one of the most important topics in frontend interview. It is important to get a good understanding of how to use Promise, how it is implemented, its internal states & value, how to use its related APIs & how these APIs are implemented.

- Promise , Promise.resolve, Promise.reject, Promise.prototype.catch, Promise.prototype.then — https://bigfrontend.dev/problem/create-your-own-Promise
- Promise.all() — https://bigfrontend.dev/problem/implement-Promise-all
- Promise.any — https://bigfrontend.dev/problem/implement-Promise-any
- Promise.allSettled() — https://bigfrontend.dev/problem/implement-Promise-allSettled
- Promise.race() — https://bigfrontend.dev/problem/implement-Promise-race
- Promise.prototype.finally — [https://bigfrontend.dev/problem/implement-Promise-prototype-finallyhttps://bigfrontend.dev/problem/implement-Promise-prototype-finally](https://bigfrontend.dev/problem/implement-Promise-prototype-finally)

Here are some good read:

[Promises, async/awaitEdit descriptionjavascript.info](https://javascript.info/async)

[Promise - JavaScript | MDNThe Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting…developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

I previously wrote an article about how to implement all of above. Go check it out.

[How to implement your own Promise and related APIs.In this article, I’d like to walk you through a simplified implementation of ES6 Promise and its related methods.medium.com](https://medium.com/@FrontendJirachi/how-to-implement-your-own-promise-and-promise-related-methods-race-any-all-allsettled-then-b982034ff830)

## Fetch API

Once you get a good handle of the promise, it would be trivial to understand how to use fetch API, fetch API is mostly used in interviews where you are expected to write a component(mostly react component). You should know how to use it, understand that it returns a promise, understand how to chain the promises. Error handling is also important.

```
fetch('http://example.com/movies.json')
  .then((response) => response.json())
  .then((data) => console.log(data))
  .catch(err => console.log(err));
```

Here are some good resources to get started.

[FetchEdit descriptionjavascript.info](https://javascript.info/fetch)

[Using the Fetch API - Web APIs | MDNThe Fetch API provides a JavaScript interface for accessing and manipulating parts of the protocol, such as requests…developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)

## Practice the following interview questions for Math & Date

Brush up on the basics of JS Date API & Math API here:

[Date - JavaScript | MDNA JavaScript date is fundamentally specified as the number of milliseconds that have elapsed since the ECMAScript…developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

For Date APIs, I think it is useful to know the following:

- Date.prototype.getDate
- Date.prototype.getDay
- Date.prototype.getFullYear
- Date.prototype.getHours
- Date.prototype.getMinutes
- Date.prototype.getMonth
- Date.prototype.getSeconds
- Date.prototype.getMilliSeconds

Understand that the results from above APIs are specific to your local time, and their UTC equivalents are:

- Date.prototype.getUTCDate
- Date.prototype.getUTCDay
- Date.prototype.getUTCFullYear
- Date.prototype.getUTCHours
- Date.prototype.getUTCMinutes
- Date.prototype.getUTCMonth
- Date.prototype.getUTCSeconds
- Date.prototype.getUTCMilliSeconds

There are also equivalent APIs to set the Date. Just replace get with set.

Date.now() & Date.prototype.getTime(), Date.prototype.toISOString() are some other useful Date APIs.

[Math - JavaScript | MDNUnlike many other global objects, Math is not a constructor. All properties and methods of Math are static. You refer…developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)

For math APIs, I think it is probably useful to know how to use:

- Math.floor
- Math.ceil
- Math.abs
- Math.max, Math.min,
- Math.sqrt

And then dive into date & math related algorithm questions. These questions can show up both in OA, Phone interview and Onsite. The following questions are very commonly seen.

1. Implement math.sqrt() — https://bigfrontend.dev/problem/implement-Math-sqrt
2. Implement math.pow() — https://bigfrontend.dev/problem/implement-Math-pow
3. The angle between hour hand and minute hand of a clock https://bigfrontend.dev/problem/the-angle-between-hour-hand-and-minute-hand-of-a-clock
4. integer to roman numerals — https://bigfrontend.dev/problem/integer-to-roman
5. roman numerals to integer — https://bigfrontend.dev/problem/roman-numerals-to-integer

Above is my plan for Week-2 interview prep. Stay tuned for Week — 3 plan where we practice the following:

- DOM APIs
- BOM APIs
- Events
- Storage