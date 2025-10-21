**Theme:** Advanced functions - constructor vs factory; prototypes & inheritance; week review
**Style:** Live‑code small domain (e.g., `Animal -> Dog/Cat`) with shared prototype methods.

## Learning Goals

- Implement a **constructor** function and a **factory** function for similar data.
- Add methods on a prototype so all instances share behavior.
- Create a simple inheritance chain and verify `instanceof` and method lookup.

## Live‑Coding Demo Checklist

- Constructor + prototype method:
  ```js
  function Animal(name) {
    this.name = name;
  }
  Animal.prototype.speak = function () {
    return this.name + " makes a noise";
  };
  ```
- Factory for similar shape:
  ```js
  const makeAnimal = (name) => ({ name, speak: () => name + " says hi" });
  ```
- Inheritance:
  ```js
  function Dog(name) {
    Animal.call(this, name);
  }
  Dog.prototype = Object.create(Animal.prototype);
  Dog.prototype.constructor = Dog;
  Dog.prototype.speak = function () {
    return this.name + " barks";
  };
  ```

## Assessment

**Day 5 - Graded In‑Class Assignment: JS Fundamentals Mini‑Build (Prototypes & Inheritance).**
(See assignment sheet.)
