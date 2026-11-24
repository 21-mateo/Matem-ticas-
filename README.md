<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <title>Quiz de Matemáticas</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0; padding: 0;
      background: #f0f0f0;
      color: #222;
    }
    header {
      background: #008000;
      color: white;
      padding: 15px 20px;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    header h1 {
      margin: 0;
    }
    nav ul {
      list-style: none;
      padding: 0;
      margin: 10px 0 0;
      display: flex;
      gap: 20px;
    }
    nav a {
      color: #a8d0e6;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    section {
      max-width: 720px;
      margin: 20px auto;
      background: white;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }
    h2 {
      color: #006400;
      margin-top: 0;
    }
    .quiz-question {
      margin-bottom: 18px;
    }
    .quiz-question h3 {
      margin-bottom: 8px;
    }
    .quiz-options label {
      display: block;
      cursor: pointer;
      margin-bottom: 6px;
      padding: 7px 12px;
      border: 1px solid #ccc;
      border-radius: 5px;
      transition: background 0.3s;
    }
    .quiz-options input[type="radio"] {
      margin-right: 10px;
      cursor: pointer;
    }
    .quiz-options label:hover {
      background: #a8d0e6;
    }
    button {
      background: #008000;
      color: white;
      border: none;
      padding: 12px 20px;
      font-size: 16px;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s;
      margin-top: 20px;
      display: block;
    }
    button:hover {
      background: #005000;
    }
    #result {
      margin-top: 25px;
      font-size: 20px;
      font-weight: 600;
      color: #007f00;
    }
    footer {
      text-align: center;
      font-size: 14px;
      color: #666;
      margin: 50px 0 20px 0;
    }
  </style>
</head>
<body>

<header>
  <h1>Quiz de Matemáticas</h1>
  <nav>
    <ul>
      <li><a href="#inicio">Inicio</a></li>
      <li><a href="#interactivo">Quiz</a></li>
      <li><a href="#fuentes">Fuentes</a></li>
    </ul>
  </nav>
</header>

<section id="inicio">
  <h2>Bienvenida</h2>
  <p>Pon a prueba tus conocimientos matemáticos con estas 10 preguntas.</p>
</section>

<section id="interactivo">
  <h2>Quiz de Matemáticas</h2>
  <form id="quizForm">

    <div class="quiz-question">
      <h3>1. ¿Cuánto es 7 x 8?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q1" value="a" required>a) 54</label>
        <label><input type="radio" name="q1" value="b">b) 56</label>
        <label><input type="radio" name="q1" value="c">c) 58</label>
      </div>
    </div>

    <div class="quiz-question">
      <h3>2. ¿Cuál es el valor aproximado de π?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q2" value="a" required>a) 2.14</label>
        <label><input type="radio" name="q2" value="b">b) 3.14</label>
        <label><input type="radio" name="q2" value="c">c) 4.13</label>
      </div>
    </div>

    <div class="quiz-question">
      <h3>3. ¿Qué resultado tiene (5 + 3) x 2?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q3" value="a" required>a) 16</label>
        <label><input type="radio" name="q3" value="b">b) 18</label>
        <label><input type="radio" name="q3" value="c">c) 20</label>
      </div>
    </div>

    <div class="quiz-question">
      <h3>4. ¿Cuál es la raíz cuadrada de 81?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q4" value="a" required>a) 8</label>
        <label><input type="radio" name="q4" value="b">b) 9</label>
        <label><input type="radio" name="q4" value="c">c) 10</label>
      </div>
    </div>

    <div class="quiz-question">
      <h3>5. Si un triángulo tiene base 10 cm y altura 4 cm, ¿cuál es su área?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q5" value="a" required>a) 40 cm²</label>
        <label><input type="radio" name="q5" value="b">b) 20 cm²</label>
        <label><input type="radio" name="q5" value="c">c) 14 cm²</label>
      </div>
    </div>

    <div class="quiz-question">
      <h3>6. ¿Cuál es la fórmula para calcular el perímetro de un rectángulo?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q6" value="a" required>a) P = base + altura</label>
        <label><input type="radio" name="q6" value="b">b) P = 2 x (base + altura)</label>
        <label><input type="radio" name="q6" value="c">c) P = base x altura</label>
      </div>
    </div>

    <div class="quiz-question">
      <h3>7. ¿Cuál es el resultado de 2³?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q7" value="a" required>a) 6</label>
        <label><input type="radio" name="q7" value="b">b) 8</label>
        <label><input type="radio" name="q7" value="c">c) 9</label>
      </div>
    </div>

    <div class="quiz-question">
      <h3>8. ¿Qué es un número primo?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q8" value="a" required>a) Un número divisible solo por 1 y por sí mismo</label>
        <label><input type="radio" name="q8" value="b">b) Un número par</label>
        <label><input type="radio" name="q8" value="c">c) Un número mayor que 100</label>
      </div>
    </div>

    <div class="quiz-question">
      <h3>9. ¿Qué representa la pendiente en una función lineal?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q9" value="a" required>a) La ordenada al origen</label>
        <label><input type="radio" name="q9" value="b">b) La inclinación o tasa de cambio</label>
        <label><input type="radio" name="q9" value="c">c) El punto máximo</label>
      </div>
    </div>

    <div class="quiz-question">
      <h3>10. ¿Cuál es la fórmula del área de un círculo?</h3>
      <div class="quiz-options">
        <label><input type="radio" name="q10" value="a" required>a) π x radio</label>
        <label><input type="radio" name="q10" value="b">b) 2 x π x radio</label>
        <label><input type="radio" name="q10" value="c">c) π x radio²</label>
      </div>
    </div>

    <button type="submit">Enviar respuestas</button>
  </form>

  <div id="result"></div>
</section>

<section id="fuentes">
  <h2>Fuentes</h2>
  <ul>
    <li><a href="https://es.wikipedia.org/wiki/Matem%C3%A1ticas" target="_blank" rel="noopener noreferrer">Wikipedia - Matemáticas</a></li>
    <li><a href="https://www.universoformulas.com/matematicas/" target="_blank" rel="noopener noreferrer">Universo Fórmulas - Matemáticas</a></li>
  </ul>
</section>

<footer>
  <p>Proyecto desarrollado por estudiante de secundaria técnica &copy; 2026</p>
</footer>

<script>
  const respuestasCorrectas = {
    q1: 'b', q2: 'b', q3: 'a', q4: 'b', q5: 'b',
    q6: 'b', q7: 'b', q8: 'a', q9: 'b', q10: 'c'
  };

  const form = document.getElementById('quizForm');
  const result = document.getElementById('result');

  form.addEventListener('submit', e => {
    e.preventDefault();
    let score = 0;
    for (let i = 1; i <= 10; i++) {
      const userAnswer = form['q'+i].value;
      if (userAnswer === respuestasCorrectas['q'+i]) score++;
    }
    let msg = `Obtuviste ${score} de 10 respuestas correctas. `;
    if (score === 10) msg += "¡Perfecto! Eres un experto en matemáticas.";
    else if (score >= 7) msg += "Muy buen trabajo.";
    else if (score >= 4) msg += "Está bien, sigue mejorando.";
    else msg += "Necesitas estudiar más.";
    result.textContent = msg;
  });
</script>

</body>
</html>

