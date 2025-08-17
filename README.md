# GATE ECE MCQ Builder

A simple **single-page quiz app** to practice GATE ECE-style MCQs with proper **marking scheme, explanations, and shortcuts**.

## ✨ Features

* Paste your **prompt (20Q test)** into the textarea → generates quiz automatically.
* Each question appears as a **card** with:

  * **Question text**
  * **4 options (A–D)**
  * **Answer section (reveals after attempt)** → correct answer, explanation, shortcut, level, year.
* **Marking Scheme:**

  * **1-mark Q** → +1 if correct, −1/3 if wrong.
  * **2-mark Q** → +2 if correct, −2/3 if wrong.
* **Score counter** updates live.
* Responsive, clean UI (cards, grid layout).
* Reset quiz anytime.

## 📝 Input Format

Paste MCQs in this structure:

```
### Topic MCQ Test

***

Q1. Question text  
(A) Option1  
(B) Option2  
(C) Option3  
(D) Option4  

***

...

## Answer Key & Explanations

Q1 → Ans: B | GATE 2019 | Exp: Stepwise explanation... | Shortcut: Fast trick... | Level: Easy | Marks:1  
Q2 → Ans: C | New Q | Exp: ... | Shortcut: ... | Level: Moderate | Marks:2  
```

* **Questions**: separated by `***` blocks.
* **Answer Key**: one line per question with → `Ans`, `Exp`, `Shortcut`, `Level`, `Year`, `Marks`.

## ⚡ How Scoring Works

* **Correct answer:** +1 or +2 (depending on marks).
* **Wrong answer:** −1/3 (for 1M) or −2/3 (for 2M).
* **Score is updated instantly** after each attempt.

## 🚀 Usage

1. Open `index.html` in a browser.
2. Paste your MCQ prompt.
3. Click **Build Quiz**.
4. Attempt questions and track your score.

## 📂 Project Structure

* `index.html` → full app (HTML, CSS, JS in one file).

## 🔮 Future Improvements

* Auto-detect marks (1M/2M) from GATE PYQs.
* Timer per quiz.
* Export results (CSV/PDF).
