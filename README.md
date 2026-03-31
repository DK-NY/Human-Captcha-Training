# Handwritten CAPTCHA Training Tool

A **web-based handwritten CAPTCHA training platform** designed to improve recognition of handwritten characters in a case-insensitive manner, with analytics for self-assessment.

---

## Features

1. **User Profile Input**
   - Users enter their name before starting the training session.
   - Analytics are personalized for each user.

2. **Handwritten CAPTCHA Generation**
   - Random 5-character CAPTCHAs using **handwritten-style fonts**: Indie Flower, Patrick Hand, Caveat.
   - Visually confusing characters (`0`, `O`, `I`, `l`, `1`) removed for clarity.
   - CAPTCHAs include random rotation, vertical displacement, font size variation, and occluding lines for realistic handwriting simulation.

3. **Difficulty Levels**
   - Users select from **Easy, Intermediate, or Hard**.
   - Difficulty affects rotation, vertical displacement, and number of occluding lines.

4. **Case-Insensitive Validation**
   - User input is validated regardless of uppercase or lowercase letters.

5. **Trial Tracking and Analytics**
   - Each session consists of **20 trials**.
   - After the session, analytics display:
     - Total trials
     - Correct answers
     - Incorrect answers
     - Accuracy percentage
   - Incorrectly answered CAPTCHAs are listed for review to facilitate learning.

6. **Keyboard Support**
   - Press **Enter** in the user name input to start training.
   - Press **Enter** in the CAPTCHA input to submit answers.

7. **Interactive UI**
   - Visual feedback for correct (✅) and incorrect (❌) answers.
   - Input box resets automatically after each trial.

---

## Usage

1. Open `index.html` in a modern web browser.
2. Enter your name and click **Start Training** (or press Enter).
3. Type the characters shown in the CAPTCHA and click **Submit** (or press Enter).
4. The next CAPTCHA generates automatically after a short delay.
5. After 20 trials, the **Training Analytics** section appears with incorrect answers for review.

---

## Technical Details

- **Languages & Libraries**
  - HTML5, CSS3, JavaScript
  - Google Fonts API for handwritten fonts

- **CAPTCHA Generation Logic**
  - Randomly selects characters from `ABCDEFGHJKLMNPQRSTUVWXYZ23456789`.
  - Applies random font, rotation, vertical displacement, and color per character.
  - Adds occluding lines proportional to difficulty.

- **Data Handling**
  - Tracks total trials, correct answers, and incorrect answers in memory.
  - Generates analytics at the end of the session.
  - Stores incorrect CAPTCHA answers for user review.

- **Accessibility**
  - Keyboard support for efficient training.
  - Visual indicators for correctness.

---

## Future Enhancements

- Display a **per-trial progress chart** to visualize performance over time.
- Highlight incorrect characters in the CAPTCHA canvas for immediate feedback.
- Allow **custom session length** and **dynamic CAPTCHA length**.
- Persist analytics for multiple sessions using local storage or backend integration.

---

## Screenshot (Placeholder)

![Screenshot](screenshot.png)

---

This tool is **ideal for human training or machine learning experiments** in recognizing handwritten characters under controlled difficulty levels.
