<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Quiz Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      padding: 20px;
      background-color: #f9f9f9;
      color: #333;
    }
    form {
      max-width: 800px;
      margin: auto;
      padding: 20px;
      background: white;
      border: 1px solid #ddd;
      border-radius: 8px;
    }
    h1 {
      text-align: center;
    }
    .question {
      margin-bottom: 20px;
    }
    .question label {
      display: block;
      margin-bottom: 8px;
      font-weight: bold;
    }
    button {
      display: block;
      width: 100%;
      padding: 10px;
      font-size: 16px;
      color: white;
      background-color: #007BFF;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #0056b3;
    }
    .result {
      margin-top: 20px;
      font-size: 18px;
      font-weight: bold;
      text-align: center;
      color: #007BFF;
    }
  </style>
</head>
<body>
  <form id="quizForm">
    <h1>English Grammar Quiz</h1>
    <p>Each question is worth 10 points. The total score is 100 points. Please enter your email below to begin.</p>

    <!-- Email Field -->
    <div class="question">
      <label for="email">Enter your email:</label>
      <input type="email" id="email" name="email" placeholder="example@example.com" required>
    </div>

    <!-- Questions -->
    <div class="question">
      <label>1. David was surprised to learn that frogs were primarily carnivorous, he had assumed that they mostly ate plants and vegetables.</label>
      <input type="radio" name="q1" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q1" value="B"> B. carnivorous, he had assumed,<br>
      <input type="radio" name="q1" value="C"> C. carnivorous (he had assumed<br>
      <input type="radio" name="q1" value="D"> D. carnivorous; he had assumed
    </div>

    <div class="question">
      <label>2. A synthesizer - an entirely electronic musical instrument: can usually be categorized into either an "East Coast" or a "West Coast" design philosophy.</label>
      <input type="radio" name="q2" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q2" value="B"> B. instrument, can<br>
      <input type="radio" name="q2" value="C"> C. instrument - can<br>
      <input type="radio" name="q2" value="D"> D. instrument; can
    </div>

    <div class="question">
      <label>3. There are a wide variety of modern dance forms and styles to enjoy. That's one reason my hometown has many different dance studios.</label>
      <input type="radio" name="q3" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q3" value="B"> B. enjoy that's<br>
      <input type="radio" name="q3" value="C"> C. enjoy, that's<br>
      <input type="radio" name="q3" value="D"> D. enjoy (that's
    </div>

    <div class="question">
      <label>4. A professional long-distance runners life revolves around his or her workout schedule, sleep routine, and dietary needs.</label>
      <input type="radio" name="q4" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q4" value="B"> B. runner<br>
      <input type="radio" name="q4" value="C"> C. runner's<br>
      <input type="radio" name="q4" value="D"> D. runners'
    </div>

    <div class="question">
      <label>5. Though the words "vintage" and "classic" are often applied interchangeably, there is a subtle difference: "vintage" has a primary reference to age, while "classic" can add an additional connotation of elegance.</label>
      <input type="radio" name="q5" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q5" value="B"> B. difference, "vintage"<br>
      <input type="radio" name="q5" value="C"> C. difference ("vintage"<br>
      <input type="radio" name="q5" value="D"> D. difference, so "vintage"
    </div><div class="question">
      <label>6. Musicians should carefully craft a strategy for their online streaming - the ability for their music to be heard instantly via the internet through a computer or mobile device) to achieve maximum popularity.</label>
      <input type="radio" name="q6" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q6" value="B"> B. streaming (the ability<br>
      <input type="radio" name="q6" value="C"> C. streaming. The ability<br>
      <input type="radio" name="q6" value="D"> D. streaming; the ability
    </div>

    <div class="question">
      <label>7. Alvin is struggling in math class this year; and there are many topics in Precalculus that he finds both challenging and frustrating.</label>
      <input type="radio" name="q7" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q7" value="B"> B. this year (there are<br>
      <input type="radio" name="q7" value="C"> C. this year, there are<br>
      <input type="radio" name="q7" value="D"> D. this year; there are
    </div>

    <div class="question">
      <label>8. Surfing (riding the waves on a wooden or plastic board) gained much of its' popularity in the 1950s and 60s in Hawaii, California, and Australia.</label>
      <input type="radio" name="q8" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q8" value="B"> B. much of its popularity<br>
      <input type="radio" name="q8" value="C"> C. much of it's popularity<br>
      <input type="radio" name="q8" value="D"> D. much of their popularity
    </div>

    <div class="question">
      <label>9. The art exhibit's brochure read like a "who's who" of famous Italian artists;Michelangelo, Raphael, Leonardo da Vinci…</label>
      <input type="radio" name="q9" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q9" value="B"> B. artists,Michelangelo<br>
      <input type="radio" name="q9" value="C"> C. artists:Michelangelo<br>
      <input type="radio" name="q9" value="D"> D. artists (Michelangelo
    </div>

    <div class="question">
      <label>10. Anyone who has had siblings - younger or older, brother or sister) will know that they are, at various times, a source of both great joy and great frustration.</label>
      <input type="radio" name="q10" value="A" required> A. [NO CHANGE]<br>
      <input type="radio" name="q10" value="B"> B. a sibling. Younger<br>
      <input type="radio" name="q10" value="C"> C. a sibling, younger<br>
      <input type="radio" name="q10" value="D"> D. a sibling (younger
    </div>

    <button type="button" onclick="calculateScore()">Submit Quiz</button>
  </form>

  <div class="result" id="result"></div>

  <script>
    const correctAnswers = {
      q1: 'D',
      q2: 'C',
      q3: 'A',
      q4: 'C',
      q5: 'A',
      q6: 'B',
      q7: 'D',
      q8: 'B',
      q9: 'C',
      q10: 'D',
      q11: 'A',
      q12: 'C'
    };

    function calculateScore() {
      const form = document.getElementById('quizForm');
      const resultDiv = document.getElementById('result');
      const email = form.email.value;

      if (!email) {
        alert('Please enter your email before submitting the quiz.');
        return;
      }

      let score = 0;

      Object.keys(correctAnswers).forEach(question => {
        const userAnswer = form[question]?.value;
        if (userAnswer === correctAnswers[question]) {
          score += 10;
        }
      });

      resultDiv.textContent = Your total score is: ${score}/100;
    }
  </script>
</body>
</html>
