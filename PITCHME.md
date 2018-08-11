## Functional Programming

>DevGrid
>leonardo()

---

### There isn't a single definition

>Is more like a coding style besides language features


### Why are we talking about functional programming now?

---

### Most popular functional p.l.
![PL](/assets/functional_lg.jpg)

---

### Is definetely a old thing.

> Why it is becoming more popular?

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

> Never change your state, always return a new one

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

### React and Redux
> React dumb components are pure function
```javascript
  Import React from 'react';
  const dumbComponent = (props) => {
    return (
      <div> // would use <React.fragment> here
        <h1>Dumb Component</h1>
        <h2>I am dumb, but I afm pure</h2>
        <p> { props.text } </p>
      </div>
    )
  };
  export default dumbComponent;
```

---

##### Reducers (free monad)
>

---
