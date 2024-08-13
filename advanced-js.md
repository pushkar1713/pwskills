Problem 1 : Create an object constructor Person that takes name and age as parameters and initializes them. Also, add a method sayHello to greet the person.

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  sayHello() {
    console.log("hello " + this.name);
  }
}

const person1 = new Person("pushkar", 20);
person1.sayHello();
```

Problem 2 : Create a constructor Employee that inherits from the Person constructor of problem 1. Add an additional property designation and a method getDetails to display the employee details.

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  sayHello() {
    console.log("hello " + this.name);
  }
}

class Employee extends Person {
  constructor(name, age, designation) {
    super(name, age);
    this.designation = designation;
  }
  getDetails() {
    console.log("name : " + this.name);
    console.log("age : " + this.age);
    console.log("designation : " + this.designation);
  }
}

const employee1 = new Employee("pushkar", 20, "teacher");
employee1.getDetails();
```

Problem 3 : Create an object Calculator with methods add, subtract, multiply, and divide Demonstrate the usage of this within these methods such that method chaining of add, subtract, multiply and divide is possible.

```javascript
class Calculator {
  constructor(value) {
    this.x = value;
  }

  add(value) {
    this.x += value;
    return this;
  }

  subtract(value) {
    this.x -= value;
    return this;
  }

  multiply(value) {
    this.x *= value;
    return this;
  }

  divide(value) {
    if (value === 0) {
      throw new Error("Division by zero is not allowed");
    }
    this.x /= value;
    return this;
  }

  getResult() {
    return this.x;
  }
}

const demo = new Calculator(1);
demo.add(1).subtract(3).multiply(10).divide(2).getResult();
console.log(demo);
```

Problem 4 : Define a base class Shape with a method draw. Create two subclasses Circle and Rectangle that override the draw method. Demonstrate polymorphism using instances of these classes.

```javascript
class shape {
  draw() {
    console.log("the shape is drawn");
  }
}

class circle extends shape {
  draw() {
    console.log("the circle is drawn");
  }
}

class rectangle extends shape {
  draw() {
    console.log("the rectangle is drawn");
  }
}

const circle1 = new circle();
const rectangle1 = new rectangle();
circle1.draw();
rectangle1.draw();
```

Problem 5: Create a simple polyfill for the Array.includes method by the name of customIncludes.

```javascript
if (!Array.prototype.customIncludes) {
  Array.prototype.customIncludes = function (searchElement, fromIndex) {
    if (this == null) {
      throw new TypeError('"this" is null or not defined');
    }

    var o = Object(this);
    var len = o.length >>> 0;

    if (len === 0) {
      return false;
    }

    var n = fromIndex | 0;
    var k = Math.max(n >= 0 ? n : len + n, 0);

    while (k < len) {
      if (o[k] === searchElement) {
        return true;
      }
      k++;
    }

    return false;
  };
}

// Example usage:
var arr = [1, 2, 3, 4, 5];
console.log(arr.customIncludes(3)); // true
console.log(arr.customIncludes(6)); // false
console.log(arr.customIncludes(3, 3)); // false
```
