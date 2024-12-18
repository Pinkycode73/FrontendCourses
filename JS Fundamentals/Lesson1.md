### **Lesson: Basics of JavaScript**

#### **1. Data Types**
In JavaScript, there are **7 primitive data types**:
1. **Number**: Represents both integer and floating-point numbers.
   ```javascript
   let age = 25;       // integer
   let price = 19.99;  // floating point
   ```
2. **String**: Represents a sequence of characters.
   ```javascript
   let name = "John Doe";  // String with double quotes
   let greeting = 'Hello'; // String with single quotes
   ```
3. **Boolean**: Represents a true or false value.
   ```javascript
   let isActive = true;
   let isCompleted = false;
   ```
4. **Undefined**: A variable that has been declared but not assigned a value.
   ```javascript
   let color;
   console.log(color);  // undefined
   ```
5. **Null**: Represents the intentional absence of any value.
   ```javascript
   let value = null;
   console.log(value);  // null
   ```
6. **Symbol**: A unique, immutable data type used for creating unique identifiers.
   ```javascript
   let symbol = Symbol('description');
   ```
7. **BigInt**: Represents integers with arbitrary precision.
   ```javascript
   let bigNumber = 9007199254740991n;  // BigInt
   ```

---

#### **2. Variables**
Variables are used to store values. You can declare them using:
- **`var`** (old way, function-scoped)
- **`let`** (modern way, block-scoped)
- **`const`** (used for constants, block-scoped)

```javascript
let name = "Alice";  // Block-scoped variable
const age = 30;      // Constant, cannot be reassigned
var city = "Paris";  // Function-scoped (use let/const instead)
```

---

#### **3. Operators**
Operators are used to perform operations on variables and values.

- **Arithmetic Operators**: Perform basic math operations.
  ```javascript
  let a = 10;
  let b = 5;
  console.log(a + b);  // 15 (addition)
  console.log(a - b);  // 5  (subtraction)
  console.log(a * b);  // 50 (multiplication)
  console.log(a / b);  // 2  (division)
  console.log(a % b);  // 0  (modulus, remainder)
  console.log(a ** b); // 100000 (exponentiation)
  ```

- **Comparison Operators**: Compare values and return a boolean (`true` or `false`).
  ```javascript
  console.log(10 > 5);   // true
  console.log(10 < 5);   // false
  console.log(10 === 10); // true (strict equality)
  console.log(10 == '10');  // true (loose equality, compares after type coercion)
  console.log(10 !== 5);  // true (not equal)
  ```

- **Logical Operators**: Used to combine boolean values.
  ```javascript
  let x = true;
  let y = false;
  console.log(x && y);  // false (AND)
  console.log(x || y);  // true  (OR)
  console.log(!x);      // false (NOT)
  ```

---

#### **4. Loops**
Loops allow you to repeat a block of code multiple times.

- **For loop**: Repeats a block of code a specific number of times.
  ```javascript
  for (let i = 0; i < 5; i++) {
      console.log(i); // Output: 0, 1, 2, 3, 4
  }
  ```

- **While loop**: Continues while a condition is `true`.
  ```javascript
  let i = 0;
  while (i < 5) {
      console.log(i);  // Output: 0, 1, 2, 3, 4
      i++;
  }
  ```

- **Do...while loop**: Executes the block of code once and then checks the condition.
  ```javascript
  let i = 0;
  do {
      console.log(i);  // Output: 0, 1, 2, 3, 4
      i++;
  } while (i < 5);
  ```

---

#### **5. Conditionals**
Conditionals allow you to execute code based on certain conditions.

- **if statement**: Executes a block of code if the condition is `true`.
  ```javascript
  let age = 20;
  if (age >= 18) {
      console.log("You are an adult.");
  }
  ```

- **else statement**: Executes a block of code if the condition is `false`.
  ```javascript
  let age = 16;
  if (age >= 18) {
      console.log("You are an adult.");
  } else {
      console.log("You are a minor.");
  }
  ```

- **else if statement**: Used for multiple conditions.
  ```javascript
  let score = 75;
  if (score >= 90) {
      console.log("A grade");
  } else if (score >= 70) {
      console.log("B grade");
  } else {
      console.log("C grade");
  }
  ```

- **switch statement**: Used for multiple possible outcomes.
  ```javascript
  let day = 3;
  switch (day) {
      case 1:
          console.log("Monday");
          break;
      case 2:
          console.log("Tuesday");
          break;
      case 3:
          console.log("Wednesday");
          break;
      default:
          console.log("Invalid day");
  }
  ```

- **Ternary operator**: A shorthand for `if` and `else`.
  ```javascript
  let age = 18;
  let result = (age >= 18) ? "Adult" : "Minor";
  console.log(result);  // Output: "Adult"
  ```

---

#### **6. Functions**
Functions are blocks of code designed to perform a particular task.

- **Function Declarations**: You can declare a function with a name.
  ```javascript
  function greet(name) {
      console.log("Hello, " + name);
  }
  greet("Alice");  // Output: Hello, Alice
  ```

- **Function Expressions**: Functions can also be defined as expressions and assigned to variables.
  ```javascript
  let greet = function(name) {
      console.log("Hello, " + name);
  };
  greet("Bob");  // Output: Hello, Bob
  ```

- **Arrow Functions**: A shorter syntax for writing functions (especially useful for callbacks).
  ```javascript
  const greet = (name) => {
      console.log("Hello, " + name);
  };
  greet("Charlie");  // Output: Hello, Charlie
  ```

---

### **Practice Exercises**
1. **Data Types**: Create variables for each data type (e.g., a number, string, boolean, etc.) and log them to the console.
2. **Loops**: Write a `for` loop that logs the numbers from 1 to 10.
3. **Conditionals**: Write a program that checks if a number is even or odd.
4. **Functions**: Create a function that takes two numbers and returns their sum.

By practicing these concepts, you'll build a strong foundation for understanding JavaScript and its core features!