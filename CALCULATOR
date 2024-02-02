<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Basic Calculator</title>
  <style>
    body {
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }

    #calculator {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      grid-gap: 8px;
      max-width: 300px;
    }

    #display {
      grid-column: span 4;
      height: 40px;
      font-size: 1.5rem;
      text-align: right;
      padding: 0 8px;
    }

    button {
      padding: 10px;
      font-size: 1rem;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div id="calculator">
    <div id="display"></div>
    <button onclick="clearDisplay()">C</button>
    <button onclick="appendCharacter('/')">/</button>
    <button onclick="appendCharacter('*')">*</button>
    <button onclick="appendCharacter('7')">7</button>
    <button onclick="appendCharacter('8')">8</button>
    <button onclick="appendCharacter('9')">9</button>
    <button onclick="appendCharacter('-')">-</button>
    <button onclick="appendCharacter('4')">4</button>
    <button onclick="appendCharacter('5')">5</button>
    <button onclick="appendCharacter('6')">6</button>
    <button onclick="appendCharacter('+')">+</button>
    <button onclick="appendCharacter('1')">1</button>
    <button onclick="appendCharacter('2')">2</button>
    <button onclick="appendCharacter('3')">3</button>
    <button onclick="calculateResult()">=</button>
    <button onclick="appendCharacter('0')">0</button>
    <button onclick="appendCharacter('.')">.</button>
  </div>

  <script>
    let display = document.getElementById('display');
    let expression = '';

    function appendCharacter(char) {
      expression += char;
      display.innerText = expression;
    }

    function clearDisplay() {
      expression = '';
      display.innerText = '';
    }

    function calculateResult() {
      try {
        expression = eval(expression).toString();
        display.innerText = expression;
      } catch (error) {
        display.innerText = 'Error';
      }
    }
  </script>
</body>
</html>
