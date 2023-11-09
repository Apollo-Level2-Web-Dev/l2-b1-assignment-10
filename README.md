**Level 2 Batch 1 Assignment 10**

**Unit-1**

```powershell
function divide(a, b) {
  if (b === 0) {
    throw new Error('Division by zero');
  }
  return a / b;
}
```

**Test Cases:**

1. **Valid Division**:
    - Test that the function correctly divides two positive numbers.
    - Example: **`divide(10, 2)`** should return **`5`**.
2. **Valid Division with Negative Numbers**:
    - Test that the function correctly handles division with negative numbers.
    - Example: **`divide(-10, 2)`** should return **`5`**.
3. **Division by Zero**:
    - Test that the function throws an error when attempting to divide by zero.
    - Example: **`divide(5, 0)`** should throw an **`Error`** with the message 'Division by zero'.

**Unit-2**

```jsx
function executeCallback(callback, taskText) {
  callback(taskText);
}

function myCallback(taskText) {
  console.log(`Task: ${taskText}`);
}

// Call executeCallback with a callback function and a task text

executeCallback(myCallback, "Buy groceries");
```

**Test Cases:**

1. **Callback Execution**:
    - Test that the **`executeCallback`** function correctly calls the provided callback function.
2. **Callback Execution with Task Text**:
    - Verify that the callback function is executed with the provided **`taskText`** argument.
    - Example: When **`executeCallback(callback, "Buy groceries")`** is called, ensure that the **`callback`** function is invoked with the argument "Buy groceries."

**Unit-3**

```jsx
function fetchData() {
  return new Promise((resolve, reject) => {
    // Simulate an async operation (e.g., fetching data from an API)
    setTimeout(() => {
      const data = { name: 'John', age: 30 };
      resolve(data);
    }, 1000); // Simulate a 1-second delay
  });
}
```

**Test Cases:**

**Successful Data Fetch**:

- Test that the **`fetchData`** function resolves with the correct data when the asynchronous operation is successful.
- For example, you can verify that the function resolves with **`{ name: 'John', age: 30 }`** when the Promise resolves.

**Error Handling**:

- Test how the function handles errors. You can create a modified version of **`fetchData`** that rejects the Promise with an error and test that it throws an error.
- For example, ensure that calling **`fetchData`** with a specific argument or configuration correctly rejects the Promise with an error message.

### **General Guidelines:**

- Use the Vitest or Jest framework to write and run your tests. Make sure your tests are written following the best practices.
- Comment your code as needed to explain the purpose of your tests and any significant steps you are taking.
- Ensure that your test cases are independent of each other, meaning the outcome of one test should not affect the others.
- Aim for comprehensive test coverage, testing both expected behavior and error conditions where applicable.

### **Deadline:**

- 60 marks: November 12, 2023, 11:59 PM
- 50 marks: November 13, 2023, 11:59 PM
- 30 marks: After 13th November, 11.59PM
