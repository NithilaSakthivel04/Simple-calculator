# simple calculator
## Date:26/08/25

## AIM
To create  a Simple Calculator using HTML, CSS, and JavaScript

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add  effects 
### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the simple calculator

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pastel Calculator</title>
  <style>
    body {
      font-family: "Poppins", sans-serif;
      background: linear-gradient(135deg, #ffd6e0, #e7c6ff, #caffbf, #a0c4ff);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .calculator {
      background: #fffafc;
      padding: 25px;
      border-radius: 20px;
      box-shadow: 0px 6px 15px rgba(0,0,0,0.1);
      width: 300px;
      text-align: center;
      border: 2px solid #e7c6ff;
    }
    h2 {
      color: #9d4edd;
      margin-bottom: 15px;
    }
    input, select, button {
      margin: 10px 0;
      padding: 10px;
      width: 90%;
      border: none;
      border-radius: 10px;
      font-size: 16px;
      outline: none;
      transition: 0.3s;
    }
    input {
      background: #e0f7fa;
    }
    input:focus {
      background: #b2ebf2;
    }
    select {
      background: #fff0f6;
      color: #6a0572;
    }
    button {
      background: #ffd6a5;
      color: #333;
      font-weight: bold;
      cursor: pointer;
    }
    button:hover {
      background: #ffb347;
    }
    .result {
      margin-top: 15px;
      font-weight: bold;
      font-size: 18px;
      color: #5a189a;
      background: #e9ecef;
      padding: 8px;
      border-radius: 12px;
    }
  </style>
</head>
<body>
  <div class="calculator">
    <h2>Pastel Calculator</h2>
    <input type="number" id="num1" placeholder="Enter first number">
    <input type="number" id="num2" placeholder="Enter second number">
    
    <select id="operation">
      <option value="add">Add (+)</option>
      <option value="subtract">Subtract (-)</option>
      <option value="multiply">Multiply (×)</option>
      <option value="divide">Divide (÷)</option>
    </select>
    
    <button onclick="calculate()">Calculate</button>
    <div class="result" id="result"></div>
  </div>

  <script>
    function calculate() {
      const num1 = parseFloat(document.getElementById("num1").value);
      const num2 = parseFloat(document.getElementById("num2").value);
      const operation = document.getElementById("operation").value;
      let result = "";

      if (isNaN(num1) || isNaN(num2)) {
        result = "⚠️ Please enter valid numbers.";
      } else {
        switch(operation) {
          case "add":
            result = `Result: ${num1 + num2}`;
            break;
          case "subtract":
            result = `Result: ${num1 - num2}`;
            break;
          case "multiply":
            result = `Result: ${num1 * num2}`;
            break;
          case "divide":
            result = num2 !== 0 ? `Result: ${num1 / num2}` : "⚠️ Cannot divide by zero!";
            break;
        }
      }
      document.getElementById("result").innerText = result;
    }
  </script>
</body>
</html>


## OUTPUT
<img width="1904" height="1064" alt="Screenshot 2025-08-26 175140" src="https://github.com/user-attachments/assets/01d9cb66-2a43-49c9-b687-0a0bc4128ba7" />
<img width="1919" height="1031" alt="Screenshot 2025-08-26 175202" src="https://github.com/user-attachments/assets/d4fba0c5-87f2-4a53-b4ff-91f8fb73ca0d" />



## RESULT
The program for creating simple calculator using HTML and CSS is executed successfully.
