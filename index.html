<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Интерактивный Математический Тренажер</title>
    <style>
        body { font-family: 'Segoe UI', Arial, sans-serif; background-color: #f4f7f6; margin: 0; padding: 20px; color: #333; }
        .container { max-width: 800px; margin: 0 auto; background: white; padding: 30px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); }
        h1, h2 { color: #2c3e50; text-align: center; }
        .navigation { display: flex; justify-content: center; gap: 10px; margin-bottom: 25px; flex-wrap: wrap; }
        .nav-btn { background: #3498db; color: white; border: none; padding: 10px 15px; border-radius: 6px; cursor: pointer; font-weight: bold; transition: 0.2s; }
        .nav-btn:hover { background: #2980b9; }
        .quiz-card { border: 2px solid #eef2f3; padding: 20px; border-radius: 8px; margin-top: 15px; background: #fafbfc; }
        .question { font-size: 1.2rem; font-weight: bold; margin-bottom: 15px; }
        .options-container { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; }
        .option-btn { background: white; border: 2px solid #bdc3c7; padding: 12px; border-radius: 6px; cursor: pointer; font-size: 1rem; text-align: left; transition: 0.2s; }
        .option-btn:hover { border-color: #3498db; background: #f0f7fc; }
        .correct { background-color: #2ecc71 !important; color: white; border-color: #27ae60 !important; }
        .wrong { background-color: #e74c3c !important; color: white; border-color: #c0392b !important; }
        .explanation { margin-top: 15px; padding: 15px; border-left: 5px solid #e74c3c; background: #fdf2f2; display: none; border-radius: 4px; }
        .success-msg { margin-top: 15px; padding: 15px; border-left: 5px solid #2ecc71; background: #f2fdf5; display: none; border-radius: 4px; color: #27ae60; font-weight: bold; }
        .action-container { margin-top: 20px; text-align: center; }
    </style>
</head>
<body>

<div class="container">
    <h1>Математический Тренажер</h1>
    <div class="navigation">
        <button class="nav-btn" onclick="loadQuestion('algebra8')">8 Класс: Алгебра (Квадратные уравнения)</button>
        <button class="nav-btn" onclick="loadQuestion('geometry8')">8 Класс: Геометрия (Теорема Пифагора)</button>
    </div>

    <h2 id="topic-title">Выберите тему выше</h2>

    <div class="quiz-card" id="quiz-space" style="display:none;">
        <div class="question" id="question-text">Загрузка вопроса...</div>
        <div class="options-container" id="options-box"></div>
        <div class="explanation" id="explanation-box"></div>
        <div class="success-msg" id="success-box">🎯 Правильно! Отличная работа.</div>
        <div class="action-container">
            <button class="nav-btn" style="background:#27ae60;" onclick="regenerateCurrent()">Сгенерировать другие числа</button>
        </div>
    </div>
</div>

<script>
let currentTopic = '';
let currentCorrectAnswer = null;
let currentExplanation = '';

// Функция генерации случайного числа в диапазоне
function getRandom(min, max) { return Math.floor(Math.random() * (max - min + 1)) + min; }

// Перемешивание массива вариантов ответов
function shuffle(array) { return array.sort(() => Math.random() - 0.5); }

function generateTask(topic) {
    let question = '';
    let correctAnswer = 0;
    let explanation = '';
    let wrongAnswers = [];

    if (topic === 'algebra8') {
        // Динамическое квадратное уравнение вида (x - x1)(x - x2) = 0 -> x^2 - (x1+x2)x + x1*x2 = 0
        let x1 = getRandom(1, 5);
        let x2 = getRandom(6, 10);
        let b = -(x1 + x2);
        let c = x1 * x2;
        
        question = `Найдите корни квадратного уравнения: x² ${b >= 0 ? '+ ' + b : b}x + ${c} = 0`;
        correctAnswer = `x = ${x1}; x = ${x2}`;
        explanation = `Для решения разложим уравнение на множители: (x - ${x1})(x - ${x2}) = 0. Отсюда получаем два корня: x = ${x1} и x = ${x2}. Также можно проверить через Дискриминант: D = (${b})² - 4·1·${c} = ${b*b - 4*c}.`;
        
        wrongAnswers = [
            `x = -${x1}; x = -${x2}`,
            `x = ${x1 + 1}; x = ${x2 - 1}`,
            `x = 0; x = ${c}`
        ];
    } 
    else if (topic === 'geometry8') {
        // Теорема Пифагора: египетские тройки (3k, 4k, 5k)
        let k = getRandom(1, 4);
        let a = 3 * k;
        let b = 4 * k;
        let c = 5 * k;

        question = `В прямоугольном треугольнике катеты равны ${a} см и ${b} см. Найдите длину гипотенузы.`;
        correctAnswer = `${c} см`;
        explanation = `По теореме Пифагора сумма квадратов катетов равна квадрату гипотенузы: a² + b² = c². Вычисляем: ${a}² + ${b}² = ${a*a} + ${b*b} = ${c*c}. Квадратный корень из ${c*c} равен ${c}.`;
        
        wrongAnswers = [
            `${a + b} см`,
            `${c + getRandom(1,3)} см`,
            `${c * c} см`
        ];
    }

    return { question, correctAnswer, wrongAnswers, explanation };
}

function loadQuestion(topic) {
    currentTopic = topic;
    document.getElementById('quiz-space').style.display = 'block';
    document.getElementById('explanation-box').style.display = 'none';
    document.getElementById('success-box').style.display = 'none';
    
    if(topic === 'algebra8') document.getElementById('topic-title').innerText = "Алгебра 8 класс: Квадратные уравнения";
    if(topic === 'geometry8') document.getElementById('topic-title').innerText = "Геометрия 8 класс: Теорема Пифагора";

    let task = generateTask(topic);
    currentCorrectAnswer = task.correctAnswer;
    currentExplanation = task.explanation;

    document.getElementById('question-text').innerText = task.question;
    document.getElementById('explanation-box').innerText = "❌ Неправильно. Объяснение: " + task.explanation;

    let allOptions = [...task.wrongAnswers, task.correctAnswer];
    allOptions = shuffle(allOptions);

    let optionsBox = document.getElementById('options-box');
    optionsBox.innerHTML = '';

    allOptions.forEach(option => {
        let btn = document.createElement('button');
        btn.className = 'option-btn';
        btn.innerText = option;
        btn.onclick = function() { checkAnswer(btn, option); };
        optionsBox.appendChild(btn);
    });
}

function checkAnswer(selectedBtn, selectedValue) {
    let buttons = document.querySelectorAll('.option-btn');
    buttons.forEach(b => b.disabled = true); // Блокируем клики после ответа

    if (selectedValue === currentCorrectAnswer) {
        selectedBtn.classList.add('correct');
        document.getElementById('success-box').style.display = 'block';
    } else {
        selectedBtn.classList.add('wrong');
        // Подсвечиваем правильный, чтобы пользователь сразу его видел
        buttons.forEach(b => {
            if(b.innerText === currentCorrectAnswer) b.classList.add('correct');
        });
        document.getElementById('explanation-box').style.display = 'block';
    }
}

function regenerateCurrent() {
    if(currentTopic) loadQuestion(currentTopic);
}
</script>
</body>
</html>
