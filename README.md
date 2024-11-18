<!DOCTYPE html>
<html lang="sr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kviz: Religija naroda starog Istoka</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            color: #333;
            padding: 20px;
        }
        .question {
            margin-bottom: 20px;
        }
        button {
            margin: 5px 0;
            padding: 10px 15px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            background-color: #007bff;
            color: white;
        }
        button:hover {
            background-color: #0056b3;
        }
        .result {
            font-weight: bold;
            margin-top: 10px;
        }
        .correct {
            color: green;
        }
        .wrong {
            color: red;
        }
    </style>
    <script>
        function checkAnswer(isCorrect, element) {
            const result = element.parentElement.querySelector('.result');
            if (isCorrect) {
                result.textContent = "Tačno!";
                result.className = "result correct";
            } else {
                result.textContent = "Netačno. Pokušaj ponovo.";
                result.className = "result wrong";
            }
        }
    </script>
</head>
<body>
    <h1>Kviz: Religija naroda starog Istoka</h1>
    <p>Odgovori na pitanja klikom na jedan od ponuđenih odgovora!</p>

    <!-- Pitanje 1 -->
    <div class="question">
        <p><strong>1. Koji narod je gradio zigurate kao verske građevine?</strong></p>
        <button onclick="checkAnswer(true, this)">a) Sumeri</button>
        <button onclick="checkAnswer(false, this)">b) Egipćani</button>
        <button onclick="checkAnswer(false, this)">c) Persijanci</button>
        <button onclick="checkAnswer(false, this)">d) Hetiti</button>
        <p class="result"></p>
    </div>

    <!-- Pitanje 2 -->
    <div class="question">
        <p><strong>2. Koji je bog bio glavni u egipatskoj mitologiji?</strong></p>
        <button onclick="checkAnswer(false, this)">a) Enlil</button>
        <button onclick="checkAnswer(true, this)">b) Ra</button>
        <button onclick="checkAnswer(false, this)">c) Ahura Mazda</button>
        <button onclick="checkAnswer(false, this)">d) Ishtar</button>
        <p class="result"></p>
    </div>

    <!-- Pitanje 3 -->
    <div class="question">
        <p><strong>3. Koja sveta knjiga je povezana sa persijskim Zoroastrizmom?</strong></p>
        <button onclick="checkAnswer(false, this)">a) Biblija</button>
        <button onclick="checkAnswer(true, this)">b) Avesta</button>
        <button onclick="checkAnswer(false, this)">c) Epopeja o Gilgamešu</button>
        <button onclick="checkAnswer(false, this)">d) Knjiga mrtvih</button>
        <p class="result"></p>
    </div>
</body>
</html>
