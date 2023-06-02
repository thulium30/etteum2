<!DOCTYPE html>
<html>

<head>
    <title>가위바위보 게임</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
        }

        .game-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-top: 100px;
        }

        .game-container button {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }

        .result {
            margin-top: 20px;
            font-size: 24px;
        }

        .win-theme {
            background-color: #1fc4f5;
            color: white;
        }

        .lose-theme {
            background-color: #f42095;
            color: white;
        }

        .draw-theme {
            background-color: #2DB400;
            color: white;
        }
    </style>
</head>

<body>
    <h1>가위바위보 게임</h1>
    <div class="game-container">
        <button onclick="playGame('scissors')">가위</button>
        <button onclick="playGame('rock')">바위</button>
        <button onclick="playGame('paper')">보</button>
        <p class="result" id="result"></p>
    </div>

    <script>
        function playGame(userChoice) {
            var choices = ["scissors", "rock", "paper"];
            var computerChoice;
            var randomNumber = Math.random();
            var winProbability = 1 / 13;
            var drawProbability = 3 / 13;
            var loseProbability = 9 / 13;

            if (userChoice === "scissors") {
                if (randomNumber < winProbability) {
                    computerChoice = "paper";
                    document.getElementById("result").innerHTML =
                        "이겼습니다! 컴퓨터는 " + computerChoice + "를 냈습니다.";
                    document.body.className = "win-theme";
                } else if (randomNumber < winProbability + drawProbability) {
                    computerChoice = "scissors";
                    document.getElementById("result").innerHTML =
                        "비겼습니다! 컴퓨터도 " + computerChoice + "를 냈습니다.";
                    document.body.className = "draw-theme";
                } else {
                    computerChoice = "rock";
                    document.getElementById("result").innerHTML =
                        "졌습니다! 컴퓨터는 " + computerChoice + "를 냈습니다.";
                    document.body.className = "lose-theme";
                }
            } else if (userChoice === "rock") {
                if (randomNumber < winProbability) {
                    computerChoice = "scissors";
                    document.getElementById("result").innerHTML =
                        "이겼습니다! 컴퓨터는 " + computerChoice + "를 냈습니다.";
                    document.body.className = "win-theme";
                } else if (randomNumber < winProbability + drawProbability) {
                    computerChoice = "rock";
                    document.getElementById("result").innerHTML =
                        "비겼습니다! 컴퓨터도 " + computerChoice + "를 냈습니다.";
                    document.body.className = "draw-theme";
                } else {
                    computerChoice = "paper";
                    document.getElementById("result").innerHTML =
                        "졌습니다! 컴퓨터는 " + computerChoice + "를 냈습니다.";
                    document.body.className = "lose-theme";
                }
            } else if (userChoice === "paper") {
                if (randomNumber < winProbability) {
                    computerChoice = "rock";
                    document.getElementById("result").innerHTML =
                        "이겼습니다! 컴퓨터는 " + computerChoice + "를 냈습니다.";
                    document.body.className = "win-theme";
                } else if (randomNumber < winProbability + drawProbability) {
                    computerChoice = "paper";
                    document.getElementById("result").innerHTML =
                        "비겼습니다! 컴퓨터도 " + computerChoice + "를 냈습니다.";
                    document.body.className = "draw-theme";
                } else {
                    computerChoice = "scissors";
                    document.getElementById("result").innerHTML =
                        "졌습니다! 컴퓨터는 " + computerChoice + "를 냈습니다.";
                    document.body.className = "lose-theme";
                }
            }
        }
    </script>
</body>

</html>
