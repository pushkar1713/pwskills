Q1. Write a JavaScript function called outerFunction that takes a parameter and returns an inner function. The inner function should access both the parameter of outerFunction and a variable declared within outerFunction. Demonstrate how lexical scoping allows the inner function to maintain access to these variables even after outerFunction has finished executing.

```javascript
function outerFunction(param) {
  let outerVar = "I'm from outer function";

  function innerFunction() {
    console.log("Parameter from outer function:", param);
    console.log("Variable from outer function:", outerVar);
  }

  return innerFunction;
}

// Create an instance of the inner function
let closureExample = outerFunction("Hello");

// Call the inner function after outerFunction has finished executing
closureExample();
```

Q2. Create a JavaScript program that demonstrates the basic usage of regular expressions. Write a function that takes a regex pattern and a string as input and returns true if there is a match, and false otherwise. Test the function with various patterns and strings.

```javascript
function regexCheck(regex, string) {
  if (regex.test(string)) {
    console.log("string matched");
    return true;
  } else {
    console.log("String is not in required pattern");
    return false;
  }
}
let password = /(?=(.*[0-9]))((?=.*[A-Za-z0-9])(?=.*[A-Z])(?=.*[a-z]))^.{8,}$/;
let email = /^[a-zA-Z0-9._%±]+@[a-zA-Z0-9.-]+.[a-zA-Z]{2,}$/;
regexCheck(email, "john@gmail.com");
regexCheck(password, "John1234");
```

Q3. Write a JavaScript program that demonstrates the use of character classes in regular expressions.Create a function that searches for specific character classes in a given string and returns the matches. Test the function with patterns for digits, uppercase letters, lowercase letters, and special characters.

```javascript
const patterns = {
  digits: /\d+/g,
  uppercaseLetters: /[A-Z]+/g,
  lowercaseLetters: /[a-z]+/g,
  specialCharacters: /[^a-zA-Z0-9\s]+/g,
};

const testString = "Hello123! How are YOU? 42 & Special $ymbols";

for (const [pattern, regex] of Object.entries(patterns)) {
  console.log(pattern, " : ", testString.match(regex));
}
```

Q4. Create a JavaScript program that takes a regex pattern and a string as input. Write a function that not only checks if there is a match but also extracts specific parts of the matched text using groups. Test the function with patterns that include groups to capture different parts of a date (e.g., day, month, and year) from a given string.

```javascript
function extractGroups(pattern, str) {
  const regex = new RegExp(pattern);
  const match = regex.exec(str);

  if (match) {
    console.log("Match found!");
    // Return an object with named groups if available
    if (match.groups) {
      return match.groups;
    } else {
      // Return an array of matched groups
      return match.slice(1); // slice(1) to skip the full match (index 0)
    }
  } else {
    console.log("No match found.");
    return null;
  }
}

// Test the function with a date string
const datePattern = /(?<day>\d{2})-(?<month>\d{2})-(?<year>\d{4})/;
const dateString = "Today's date is 13-08-2024.";

const result = extractGroups(datePattern, dateString);
console.log(result); // Output: { day: '13', month: '08', year: '202
```

Q5. You are building a shipping application. Write a program that takes the type of package ("standard","express", or "overnight") and uses a switch statement to calculate and print the estimated delivery time based on the package type. For example, "standard" might take 3-5 days, "express" 1-2 days, and "overnight" would be delivered the next day.

```javascript
const deliveryType = prompt(
  "Select delivery type, enter 0 for standard, 1 for express, 2 for overnight: "
);
switch (parseInt(deliveryType)) {
  case 0:
    console.log("3-5 days");
    break;

  case 1:
    console.log("1-2 days");
    break;

  case 2:
    console.log("tomorrow");
    break;

  default:
    console.log("Invalid selection");
}
```
