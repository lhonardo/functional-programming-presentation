## Functional Programming

>Leonardo

>DevGrid
---

### There isn't a single definition

>Is more like a coding style

---

### Most popular functional p.l.
![PL](/assets/functional_lg.jpg)

---

### Is a old thing.

> Why it is becoming more popular now?

---

### In general, is slow

* Is less efficient than a mutable way, like C or Java
* In the past, computers hardwares used to be less powerful
* The preference was to a paradigm more friendly to limited computer resources

---

### Cpu clock evolution
![Clock Evolution](/assets/cpu_clocks.jpg)

---

### The free lunch is over
#### (Herb Sutter - 2005)

> "Concurrency is the next major revolution in how we write software"

> Stated that microprocessor serial-processing speed is reaching a physical limit, which leads to two main consequences:

---

### The free lunch is over

* Processor manufacturers will focus on products that better support multithreading (such as multi-core processors)
* Software developers will be forced to develop massively multithreaded programs as a way to better use such processors.

---

### Most popular functional p.l.
![PL](/assets/functional_lg.jpg)

---

### Vertical scaling

* Using the principles of functional programming
* Functional programming languages offers better tools to work with concurrency
* Delivery business value

---

### Concepts

* Immutability
* Pure functions
* Closure

---

### Immutability

> It allows for a thread to act on data represented by immutable objects without worrying what other threads are up to.

> In short: immutable objects are more thread-safe than mutable objects.

---
### Programming with shared mutable state

[![video](http://img.youtube.com/vi/6YeomFAlgWg/0.jpg)](http://www.youtube.com/watch?v=6YeomFAlgWg)

---

### Pure functions

> A function that has NO side effects

```javascript
  function sum(a, b) {
    launchNuclearRocket(); // <-- side effect
    return a + b;
  };
```
---

### Closure in javascript

> Code

---

### React
> React dumb components are pure function

```javascript
  Import React from 'react';
  const dumbComponent = (props) => {
    return (
      <div>
        <h1>Dumb Component</h1>
        <h2>I am dumb, but I am pure</h2>
        <p> { props.text } </p>
      </div>
    )
  };
  export default dumbComponent;
```

---

### Redux
> Time traveling debug is only possible because immutability

```javascript
  switch (type) {
    case types.NOTES_UPDATED:
      return {
        ...state,
        notes: [payload, ...state.notes]
      }
    case types.NOTE_DELETED:
     const elementToRemove = notes.find(n => n.key === payload.key);
     notes.splice(notes.indexOf(elementToRemove), 1);
      return {
        ...state,
        notes: [...notes],
      }
    default: return state;
  }
```
---

### Difference between paradigms

> Functional programming languages encourages you to act functional

---

### Thank you!

---
