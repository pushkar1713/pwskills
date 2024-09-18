Q1. Explain the role of operators in JavaScript. Why are they essential in programming?

Ans : JavaScript Operators are symbols used to perform specific mathematical, comparison, assignment, and logical computations on operands. They are fundamental elements in JavaScript programming, allowing developers to manipulate data and control program flow efficiently. Understanding the different types of operators and how they work is important for writing effective and optimized JavaScript code.

Q2. Describe the categorization of operators in JavaScript based on their functionality. Provide examples for
each category.

Ans : There are different types of JavaScript operators:

1. Arithmetic Operators

```javascript
let a = 3;
let x = (100 + 50) * a;
```

2. Assignment Operators

```javascript
let x = 10;
x += 5;
```

3. Comparison Operators

```javascript
// equal to operator
console.log("Equal to: 2 == 2 is", 2 == 2);

// not equal operator
console.log("Not equal to: 3 != 3 is", 3 != 3);

// strictly equal to operator
console.log("Strictly equal to: 2 === '2' is", 2 === "2");

// strictly not equal to operator
console.log("Strictly not equal to: 2 !== '2' is", 2 !== "2");

// greater than operator
console.log("Greater than: 3 > 3 is", 3 > 3);

// less than operator
console.log("Less than: 2 > 2 is", 2 > 2);

// greater than or equal to operator
console.log("Greater than or equal to: 3 >= 3 is", 3 >= 3);

// less than or equal to operator
console.log("Less than or equal to: 2 <= 2 is", 2 <= 2);
```

4. Logical Operator

```javascript
const x = 5,
  y = 3;
console.log(x < 6 && y < 5);

// Output: true
```

5. Bitwise Operator

```javascript
console.log(5 & 3);
// ans 1
```

6. String Concatenation operator

```javascript
let str1 = "Hel",
  str2 = "lo";
console.log(str1 + str2);

// Output: Hello
```

Q3. Differentiate between unary, binary, and ternary operators in JavaScript. Give examples of each.

Ans : Operators can be categorized based on the number of operands they require

- Unary Oprerator : which require one operand
  examples are :

1. typeof operator
2. delete operator
3. unary plus

- Binary Operator : Which require two operands
  examples are :

1. arithmetic operators
2. comparison operators
3. assignment operators

- ternary operator : which require three operands
  examples are :

1. conditional operators

Q4. Discuss the precedence and associativity of operators in JavaScript. Why is understanding these concepts
important?

Ans : Operator precedence determines the order in which different operators are evaluated in a complex expression. Operators with higher precedence are evaluated before operators with lower precedence. This is similar to the order of operations (PEMDAS/BODMAS) in arithmetic.

Operator associativity defines the direction in which operators of the same precedence level are processed. There are two types of associativity:

Left-to-right (Left Associativity): Operators are evaluated from left to right.

Right-to-left (Right Associativity): Operators are evaluated from right to left.

we often encounter complex expressions involving multiple operators. Understanding how JavaScript determines the order of evaluation for these operators is crucial for writing correct and efficient code.

Q5. Write a JavaScript program that calculates the simple interest using the formula Simple interest =
(principal _ rate _ time) / 100.

Ans :

```javascript
// Function to calculate simple interest
function calculateSimpleInterest(principal, rate, time) {
  const simpleInterest = (principal * rate * time) / 100;
  return simpleInterest;
}

// Example usage
const principal = 1000; // Principal amount
const rate = 5; // Interest rate
const time = 2; // Time in years

const interest = calculateSimpleInterest(principal, rate, time);
console.log(`The simple interest is: ${interest}`);
```

Q6. Write a Javascript program to calculate the Body Mass Index (BMI) using the formula BMI = weight (kg)/
height \* height.

Ans :

```javascript
function BMI(weight, height) {
  const bmi = weight / (height * height);
  return bmi;
}

// Example usage
const height = 172; // in cm
const weight = 70; // in kg

const bmi = BMI(height, weight);
console.log(`The BMI is: ${bmi}`);
```

Q7. Write a program in JavaScript to calculate the area of a circle given its radius value of 10. Use appropriate
arithmetic operators.

Ans :

```javascript
function area(radius) {
  const ans = 3.14 * (radius * radius);
  return ans;
}

// Example usage
const radius = 10; // in cm

const ans = area(radius);
console.log(`The area is: ${ans}`);
```
