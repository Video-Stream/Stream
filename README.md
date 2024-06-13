<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Кликер</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
        }

        #counter {
            font-size: 2em;
            margin-bottom: 20px;
        }

        #clickButton {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            border: 5px solid black;
            background-size: cover;
            background-image: url('qw.jpg');
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div id="counter">0</div>
    <div id="clickButton" onclick="incrementCounter()"></div>

    <script>
        let counter = 0;
        function incrementCounter() {
            counter++;
            document.getElementById('counter').textContent = counter;
        }
    </script>
</body>
</html>
