# 🧩 Assembly: Endgame

A fun little React word game where you fight to save the programming world from **Assembly** taking over!  
Guess the hidden word within 8 tries — or watch one programming language vanish at a time.  
Each wrong guess eliminates a language (HTML, CSS, JS... until only Assembly remains 👀).

---

## 🚀 Features

✅ Random word selection from a list of 400+ words  
✅ Visual language "chips" that disappear after wrong guesses  
✅ Farewell messages in multiple styles (“RIP, JavaScript 💀”)  
✅ Confetti celebration when you win 🎉  
✅ Accessible ARIA labels and polite screen reader updates  
✅ "New Game" button to instantly reset and start again  
✅ Fully responsive layout

---

## 🧠 How It Works

The app picks a random word using `getRandomWord()` from the `words.js` list.  
You guess letters by clicking the on-screen keyboard.

- Correct guesses reveal the letters in the word  
- Wrong guesses knock out one language from the `languages.js` array  
- When all languages (except Assembly) are gone — game over 😭  
- When you reveal the full word — confetti time 🎊

---

## 🧩 Tech Stack

| Technology | Purpose |
|-------------|----------|
| **React** | UI framework |
| **useState** | State management for guesses and game flow |
| **clsx** | Clean conditional class handling |
| **React-Confetti** | Adds confetti celebration on win |
| **Vanilla JS logic** | Word and language mechanics |
| **Custom utilities** | Random word + random farewell text |

---

## 🖼️ Folder Structure

```pgsql
root/
│
├── AssemblyEndgame.jsx # Main game component
├── languages.js # List of programming languages
├── utils.js # Helper functions (random word + farewell)
├── words.js # Big word list (400+)
├── styles.css # Styling and animations
└── 
```

---

## 🕹️ How to Play

1. Click any letter to guess it.  
2. Each incorrect guess removes one programming language.  
3. Win by revealing all letters before they’re gone!  
4. Lose and Assembly rules the world 😈.  
5. Click **“New Game”** to start over.

---

## 💻 Installation

Clone and run locally with:

```bash
git clone https://github.com/elm042025/assembly-endgame.git
cd assembly-endgame
npm install
npm run dev
