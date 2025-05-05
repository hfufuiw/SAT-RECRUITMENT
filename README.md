<div class="question">
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
