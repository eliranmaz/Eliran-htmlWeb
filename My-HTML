<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Simple Calculator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f2f2f2;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }

    h2 {
      color: #333;
    }

    .calculator {
      background: #fff;
      padding: 20px 30px;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.1);
    }

    input, select, button {
      padding: 10px;
      margin: 10px;
      font-size: 16px;
    }

    #result {
      margin-top: 15px;
      font-size: 18px;
      color: #007BFF;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <h2>Simple Calculator</h2>

  <div class="calculator">
    <input type="number" id="num1" placeholder="Number 1">
    
    <select id="operator">
      <option value="+">+</option>
      <option value="-">−</option>
      <option value="*">×</option>
    </select>
    
    <input type="number" id="num2" placeholder="Number 2">
    
    <button onclick="calculate()">=</button>
    
    <div id="result">Result will appear here</div>
  </div>

  <script>
    function calculate() {
      const num1 = parseFloat(document.getElementById('num1').value);
      const num2 = parseFloat(document.getElementById('num2').value);
      const op = document.getElementById('operator').value;

      if (isNaN(num1) || isNaN(num2)) {
        document.getElementById('result').textContent = "Please enter valid numbers.";
        return;
      }

      let result;
      if (op === '+') result = num1 + num2;
      else if (op === '-') result = num1 - num2;
      else if (op === '*') result = num1 * num2;

      document.getElementById('result').textContent = "Result: " + result;
    }
  </script>

</body>
</html>
