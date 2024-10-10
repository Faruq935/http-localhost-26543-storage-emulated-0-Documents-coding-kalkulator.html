<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kalkulator I LOVE YOU ❤️</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .calculator {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        .calculator input {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            font-size: 20px;
            text-align: right;
            border: 2px solid #ddd;
            border-radius: 5px;
        }
        .calculator button {
            width: 23%;
            padding: 15px;
            margin: 5px;
            font-size: 18px;
            cursor: pointer;
            border: none;
            background-color: #f8f8f8;
            border-radius: 5px;
        }
        .calculator button.operation {
            background-color: #ff69b4;
            color: white;
        }
        .calculator button.equals {
            background-color: #ff4081;
            color: white;
        }
        .calculator button.clear {
            background-color: #ff1744;
            color: white;
        }
    </style>
</head>
<body>

    <div class="calculator">
        <input type="text" id="display" disabled>
        <br>
        <button onclick="appendToDisplay('1')">1</button>
        <button onclick="appendToDisplay('2')">2</button>
        <button onclick="appendToDisplay('3')">3</button>
        <button class="operation" onclick="appendToDisplay('+')">+</button>
        <br>
        <button onclick="appendToDisplay('4')">4</button>
        <button onclick="appendToDisplay('5')">5</button>
        <button onclick="appendToDisplay('6')">6</button>
        <button class="operation" onclick="appendToDisplay('-')">-</button>
        <br>
        <button onclick="appendToDisplay('7')">7</button>
        <button onclick="appendToDisplay('8')">8</button>
        <button onclick="appendToDisplay('9')">9</button>
        <button class="operation" onclick="appendToDisplay('*')">*</button>
        <br>
        <button onclick="appendToDisplay('0')">0</button>
        <button class="clear" onclick="clearDisplay()">C</button>
        <button class="equals" onclick="calculate()">=</button>
        <button class="operation" onclick="appendToDisplay('/')">/</button>
    </div>

    <script>
        function appendToDisplay(value) {
            document.getElementById('display').value += value;
        }

        function clearDisplay() {
            document.getElementById('display').value = '';
        }

        function calculate() {
            document.getElementById('display').value = "I LOVE YOU ❤️";
        }
    </script>

</body>
</html>
