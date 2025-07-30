<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>JogoTech</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Tela de Início -->
    <div class="start-screen" id="start-screen">
        <div class="start-container">
            <h1>JogoTech</h1>
            <p>Teste seus conhecimentos em tecnologia e cultura geral!</p>
            <button id="start-btn" class="primary-btn">Iniciar Jogo</button>
        </div>
    </div>

    <!-- Tela do Jogo -->
    <div class="quiz-app" id="quiz-app" style="display: none;">
        <header>
            <div class="logo">JogoTech</div>
            <div class="progress-container">
                <div class="progress-bar"></div>
                <span class="progress-text">Pergunta <span id="current-question">0</span>/<span id="total-questions">0</span></span>
            </div>
        </header>

        <main>
            <div class="question-container">
                <div class="question-box">
                    <p id="question-text">Preparado para o desafio?</p>
                    <div id="question-image"></div>
                </div>
                
                <div id="options-container" class="options-grid"></div>
            </div>

            <div class="action-area">
                <div class="score-container">
                    <span id="score-display">Pontuação: <span>0</span></span>
                    <div class="timer" id="timer">15s</div>
                </div>
                <button id="action-btn" class="primary-btn">Próxima</button>
            </div>
        </main>

        <div class="notification" id="notification"></div>
    </div>

    <!-- Tela de Resultado -->
    <div class="result-screen" id="result-screen" style="display: none;">
        <div class="result-container">
            <h2>Jogo Concluído!</h2>
            <div class="result-score" id="final-score">0/0</div>
            <div class="result-message" id="result-message"></div>
            <button id="restart-btn" class="primary-btn">Jogar Novamente</button>
            <button id="new-quiz-btn" class="secondary-btn">Novo Jogo</button>
        </div>
    </div>

    <!-- Efeitos Sonoros -->
    <audio id="correct-sound" src="sounds/correct.mp3"></audio>
    <audio id="wrong-sound" src="sounds/wrong.mp3"></audio>
    <audio id="levelup-sound" src="sounds/levelup.mp3"></audio>
    <audio id="start-sound" src="sounds/start.mp3"></audio>

    <script src="script.js"></script>
</body>
</html>
