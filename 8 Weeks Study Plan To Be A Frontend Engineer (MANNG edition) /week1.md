With hiring freeze, large-scale layoffs impacting the tech industry and a huge influx of experienced engineers on the market, stakes have never been higher. Now is probably a good time to brush up on the interview skills again. This is a consolidated 8-week study plan to prepare you for your next frontend interview, I will list out the JS basics to brush up on, the algorithm questions and projects to practice. For me, this is the list that I will follow if I end up in the same boat. 😿

Previously I wrote about frontend interview prep materials that helped me land a job at MANNG. If you are interested, you can check it out here:

[Frontend Interview Preparation MaterialsI’m consolidating a list of prep materials that helped me land the frontend engineer position at MANNG. There are tons…medium.com](https://medium.com/@FrontendJirachi/frontend-engineer-interview-prep-materials-bab267107272)

This series of articles will focus more on the logistics and the weekly plan. Without furthur due, let’s dive in.

**Week — 1**

## **Brush up on:**

- **JavaScript Data Types — https://javascript.info/data-types**
- **Js basic primitive: https://developer.mozilla.org/en-US/docs/Glossary/Primitive**
- **Prototypical inheritance — https://javascript.info/prototypes**
- **Scope & Closure — https://javascript.info/closure**

JavaScript is arguably the most important piece in the frontend interview. So take time to brush up on these basics. If it is your first time going through this practice, it will take you slightly longer, but don’t get discouraged it is normal.

## **Get familiar with ES6 syntax**

- https://www.w3schools.com/js/js_es6.asp

ES6 introduced the most features to JavaScript since JavaScript existed, get familiar with the ES6 syntax is super crucial.

## **Practice the following interview questions for Array**

**Brush up on the basics of an array here:**

**[ArraysEdit descriptionjavascript.info](https://javascript.info/array)**

**[Array methodsArrays provide a lot of methods. To make things easier, in this chapter they are split into groups. We already know…javascript.info**](https://javascript.info/array-methods)

And then dive into array algorithm questions. These questions can show up both in OA, Phone interview and Onsite. The following questions are very commonly seen.

- **Implement array’s map method, flat method, reduce method**

```js
// Map method
Array.prototype.myMap = function(callback, thisObj) {
  const result = [];
  this.forEach((...args) => {
    const index = args[1];
    result[index] = callback.apply(thisObj, args);
  })
  return result;
}
// Flat method
Array.prototype.myFlat = function(arr, depth = 1) {
  let result = []
  arr.forEach((elem) => {
    if (Array.isArray(elem) && depth > 0) {
      result = result.concat(flat(elem, depth - 1));
    } else {
      result.push(elem);
    }
  })
  return result;
}// Reduce method
Array.prototype.myReduce = function (callback, initialVal) {
  if (this.length === 0 && arguments.length === 1) {
    throw new Error('')
  }
  let accumulator = arguments.length === 1 ? this[0] : initialVal;
  let start = arguments.length === 1 ? 1 : 0;
  for (let i = start; i < this.length; i++) {
    accumulator = callback(accumulator, this[i], i, this);
  }
  return accumulator;
};
```

- **Shuffle an array** — https://bigfrontend.dev/problem/can-you-shuffle-an-array
- **Find median of two sorted array** — https://bigfrontend.dev/problem/find-median-of-2-sorted-array
- **Remove duplicates from an array** — https://bigfrontend.dev/problem/remove-duplicates-from-an-array
- **Array intersect** — https://bigfrontend.dev/problem/array-intersect
- **Merge sorted array** — https://bigfrontend.dev/problem/merge-sorted-arrays
- **Support negative array index in js** — https://bigfrontend.dev/problem/support-negative-Array-index
- **Reorder array with new indexes** — https://bigfrontend.dev/problem/reorder-array-with-new-indexes

**Practice the following interview questions for String**

Brush up on the basics of a string here:

[StringsIn JavaScript, the textual data is stored as strings. There is no separate type for a single character. The internal…javascript.info](https://javascript.info/string)

Dive into string algorithm questions:

- **Validate number string** — https://bigfrontend.dev/problem/validate-number-string-1
- **Validate parenthesis** — https://bigfrontend.dev/problem/validate-parenthesis
- **Extract anchor tag from HTML string** — https://bigfrontend.dev/problem/extract-all-anchor-elements-from-HTML-string
- **Compress a string** — https://bigfrontend.dev/problem/compress-a-string
- **Implement string.trim()** — https://bigfrontend.dev/problem/implement-String-prototype-trim
- **Longest substring with unique characters()** — https://bigfrontend.dev/problem/longest-substring-with-unique-characters
- **Implement JSON.stringify()** — https://bigfrontend.dev/problem/implement-JSON-stringify
- **Count palindromic substrings** — https://bigfrontend.dev/problem/Count-palindromic-substrings
- **Uncompress strings** — https://bigfrontend.dev/problem/uncompress-string

Above is my plan for Week-1 interview prep. Continue with Week — 2 plan where we practice the following:

- Async, promise
- Date, math, regex
- Map, Object

[8 Weeks Study Plan To Be A Frontend Engineer (MANNG edition) — Week 2The clock is ticking. I hope you have gone through the plan for week 1.medium.com](https://medium.com/@FrontendJirachi/8-weeks-study-plan-to-be-a-frontend-engineer-manng-edition-week-2-76dd08770042)