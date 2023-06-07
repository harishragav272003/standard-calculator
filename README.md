# Design of a Standard Calculator

## AIM:

To design a web application for a standard calculator.

## DESIGN STEPS:

### Step 1:


### Step 2:


### Step 3:


### Step 4:


### Step 5:

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html>
<head>
  <title>Simple Calculator</title>
  <style>
    .calculator {
      width: 200px;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      background-color: #f5f5f5;
      margin: 0 auto;
    }
    .calculator input[type="text"] {
      width: 100%;
      margin-bottom: 10px;
    }
    .calculator input[type="button"] {
      width: 48%;
      padding: 5px;
      margin-bottom: 5px;
    }
  </style>
</head>
<body>
    <h2 align = "center">Calculator </h2> 
  <div class="calculator">
    <input type="text" id="result" readonly>
    <input type="button" value="1" onclick="appendNumber(1)">
    <input type="button" value="2" onclick="appendNumber(2)">
    <input type="button" value="3" onclick="appendNumber(3)">
    <input type="button" value="4" onclick="appendNumber(4)">
    <input type="button" value="5" onclick="appendNumber(5)">
    <input type="button" value="6" onclick="appendNumber(6)">
    <input type="button" value="7" onclick="appendNumber(7)">
    <input type="button" value="8" onclick="appendNumber(8)">
    <input type="button" value="9" onclick="appendNumber(9)">
    <input type="button" value="0" onclick="appendNumber(0)">
    <input type="button" value="+" onclick="appendOperator('+')">
    <input type="button" value="-" onclick="appendOperator('-')">
    <input type="button" value="*" onclick="appendOperator('*')">
    <input type="button" value="/" onclick="appendOperator('/')">
    <input type="button" value="=" onclick="calculate()">
    <input type="button" value="Clear" onclick="clearResult()">
  </div>

  <script>
    function appendNumber(number) {
      document.getElementById("result").value += number;
    }

    function appendOperator(operator) {
      document.getElementById("result").value += operator;
    }

    function calculate() {
      var result = eval(document.getElementById("result").value);
      document.getElementById("result").value = result;
    }

    function clearResult() {
      document.getElementById("result").value = "";
    }
  </script>
</body>
</html>
```

## OUTPUT:
![image](https://github.com/harishragav272003/standard-calculator/assets/119345345/a13f5156-e01e-42ce-9eda-22e8460575f2)

## Result:
Standard Calculator using HTML , CSS executed successfully.
