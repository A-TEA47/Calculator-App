Simplest Working Calculator
This project is a basic React calculator app that performs simple arithmetic operations (addition, subtraction, multiplication, and division) on numbers entered by the user. It allows users to reset the input or the result displayed.

Features
Addition: Adds the entered number to the current total.
Subtraction: Subtracts the entered number from the current total.
Multiplication: Multiplies the current total by the entered number.
Division: Divides the current total by the entered number.
Reset Input: Clears the input field without affecting the current total.
Reset Result: Resets the total to zero.
Code Structure
App Component: The main functional component that renders the calculator interface.
useRef is used for referencing the input and result elements.
useState manages the result, which is updated with each operation.
CSS: Basic styling is defined in App.css for input fields and buttons.
Files
App.js: Contains the core logic and rendering for the calculator.
App.css: Provides styling for elements such as input fields and buttons.
How to Use
Type a number in the input field.
Click the operation button (add, subtract, multiply, divide) to perform the operation on the current total.
Use the reset buttons to clear either the input field or reset the total to zero.

```css
* {
    font-family: sans-serif;
}
input,
button {
    font-size: 20px;
    padding: 10px;
    border-radius: 5px;
}
input {
    display: block;
    margin-bottom: 20px;
}
button {
    border: 1px solid gray;
    background: whitesmoke;
    margin-right: 5px;
}
button:nth-last-child(2),
button:nth-last-child(1) {
    background: tomato;
    color: white;
}
```

Here is the app's starting code:
```jsx
import {
  useState,
  useRef
} from "react"; 
import "./App.css";

function App() { 
  const inputRef = useRef(null); 
  const resultRef = useRef(null); 
  const [result, setResult] = useState(0); 
 
  function plus(e) { 
    e.preventDefault(); 
    setResult((result) => result + Number(inputRef.current.value)); 
  }; 
 
  function minus(e) { 
  };
 
  function times(e) { 
  }; 
 
  function divide(e) { 
  };
 
  function resetInput(e) { 
  }; 
 
  function resetResult(e) { 
  }; 
 
  return ( 
    <div className="App"> 
      <div> 
        <h1>Simplest Working Calculator</h1> 
      </div> 
      <form> 
        <p ref={resultRef}> 
          {/* add the value of the current total */} 
        </p> 
        <input
          pattern="[0-9]" 
          ref={inputRef} 
          type="number" 
          placeholder="Type a number" 
        /> 
        <button onClick={plus}>add</button> 
        {/* Add the subtract button */} 
        {/* Add the multiply button */} 
        {/* Add the divide button */} 
        {/* Add the resetInput button */} 
        {/* Add the resetResult button */} 
      </form> 
    </div> 
  ); 
} 
 
export default App;
```

Your goal is to use this starting code and extend it with missing pieces to make the app behave as expected: a fully working simple calculator app.
"# Calculator-App" 
