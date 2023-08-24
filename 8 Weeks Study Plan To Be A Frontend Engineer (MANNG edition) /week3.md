For Week — 3, let’s talk about the knowledge you need to know for DOM APIs, Events and Storage and practice some algorithmic questions.

## DOM APIs

Nowadays, with frontend library/framework abstracting away the low level DOM APIs and providing wrapper API around it, you will rarely interact with them directly. But they are the fundamentals for frontend development and sometimes you may come across them in various libraries that you use for your project.

Here are some good read to get started:

[Walking the DOMThe DOM allows us to do anything with elements and their contents, but first we need to reach the corresponding DOM…javascript.info](https://javascript.info/dom-navigation)

[Searching: getElement*, querySelector*DOM navigation properties are great when elements are close to each other. What if they are not? How to get an…javascript.info](https://javascript.info/searching-elements-dom)

[Modifying the documentDOM modification is the key to creating "live" pages. Here we'll see how to create new elements "on the fly" and modify…javascript.info](https://javascript.info/modifying-document)

It is essential to understand:

- What DOM is? — Think of it as an interface/way to represent HTML/XML document as a tree with nodes. And each node is essentially an object manipulable by JavaScript.
- Know different types of DOM nodes — https://javascript.info/dom-nodes
- APIs to walk the DOM —

![img](https://miro.medium.com/v2/resize:fit:1400/1*v50Zk83VhmUJl42PDgQwNw.png)

https://javascript.info/dom-navigation

![img](https://miro.medium.com/v2/resize:fit:1400/1*YEa97Ce44eU8lvg8zi_2vw.png)

https://javascript.info/dom-navigation

- Different APIs to get DOM element — https://javascript.info/searching-elements-dom
- Understand DOM hirearchy, the root of the hierarchy is [EventTarget](https://dom.spec.whatwg.org/#eventtarget), that is inherited by [Node](https://dom.spec.whatwg.org/#interface-node), and other DOM nodes inherit from it.

![img](https://miro.medium.com/v2/resize:fit:1400/1*YwhmK4kpe0u3SFR9P79HjA.png)

https://javascript.info/basic-dom-node-properties

- Understand difference between DOM attributes & properties — https://javascript.info/dom-attributes-and-properties
- Different APIs to modify the DOM — https://javascript.info/modifying-document
- Different APIs to get element width, height and other geometry features. — https://javascript.info/size-and-scroll

Once you brush up on these basic knowledge, we can dive into algorithmic questions.

**Some of the most commonly seen questions include:**

1. Find corresponding node in two identical dom tree https://bigfrontend.dev/problem/find-corresponding-node-in-two-identical-DOM-tree
2. Next right sibling: https://bigfrontend.dev/problem/Next-Right-Sibiling
3. Previous left sibling: https://bigfrontend.dev/problem/previous-left-sibling
4. Traverse dom level by level: https://bigfrontend.dev/problem/Traverse-DOM-level-by-level
5. Create a simple store for DOM element — https://bigfrontend.dev/problem/create-a-simple-store-for-DOM-node

## Events

You probably remember from above that the root of the DOM hierarchy is [EventTarget](https://dom.spec.whatwg.org/#eventtarget), that is inherited by [Node](https://dom.spec.whatwg.org/#interface-node), and other DOM nodes inherit from it. Some good read on browser events:

[Introduction to browser eventsAn event is a signal that something has happened. All DOM nodes generate such signals (but events are not limited to…javascript.info](https://javascript.info/introduction-browser-events)

[Event reference | MDNEvents are fired to notify code of "interesting changes" that may affect code execution. These can arise from user…developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/Events)

It is important to understand:

- Different ways to assign event handlers, different types of events — https://javascript.info/introduction-browser-events https://javascript.info/event-details
- Understand event Bubbling and capturing — https://javascript.info/bubbling-and-capturing
- Understand event delegation, benefits of using event delegation — https://javascript.info/event-delegation
- How to create/dispatch custom events — https://javascript.info/dispatch-events

Once you are familiar with the above topics, try to practice the following algorithmic questions:

1. Event delegation — https://bigfrontend.dev/problem/event-delegation
2. Create an event emitter — https://bigfrontend.dev/problem/create-an-Event-Emitter

## Storage

Browser provides different mechanism to store data — cookie, localStorage, sessionStorage and indexDB. It is important to understand the pros & cons, use cases for each of these. Here is a great read:

[Storing data in the browserEdit descriptionjavascript.info](https://javascript.info/data-storage)

Practice this question once you finish the above read:

1. Local storage with expiration — https://bigfrontend.dev/problem/localStorage-with-expiration

I hope you are following along the week 3 plan so far. Stay tuned for week 4 where we discuss different sorting algorithms. We will also practice more commonly seen frontend algorithmic questions.