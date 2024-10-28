<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Интерактивная игра</title>
    <script>
        function makeChoice(choice) {
            let resultText;

            switch (choice) {
                case "1":
                    resultText = "Вы успешно убегаете!";
                    break;
                case "2":
                    resultText = "Вы сражаетесь с чудовищем и побеждаете!";
                    break;
                case "3":
                    resultText = "Чудовище вас испугалось и уходит.";
                    break;
                default:
                    resultText = "Некорректный выбор. Игра заканчивается.";
                    break;
            }

            document.getElementById("result").innerText = resultText;
        }
    </script>
</head>
<body>
    <h1>Добро пожаловать в интерактивную игру!</h1>
    <p>Выходит чудовище! Что вы будете делать?</p>
    <button onclick="makeChoice('1')">Убежать</button>
    <button onclick="makeChoice('2')">Сразиться</button>
    <button onclick="makeChoice('3')">Поговорить</button>
    
    <h2>Результат:</h2>
    <p id="result"></p>
</body>
</html>
