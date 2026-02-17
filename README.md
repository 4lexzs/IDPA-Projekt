# <p align="center">Wirtschaftsquiz - IDPA Project 🎓</p>

<p align="center">
  <img src="https://files.catbox.moe/czgpy5.gif" alt="wirtschaftsquiz gif"/>
</p>

<p align="center"><strong>Wirtschaftsquiz</strong> is an interactive platform in German for creating and taking quizzes with a UI/UX-focused interface, developed as part of an Individual Practical Work (IDPA). The project focuses on testing knowledge in the field of economics, but thanks to its flexible structure, it can be used for any thematic tests.</p>

<p align="center"><strong>This README is also available in <a href="/README_de.md">Deutsch</a> and <a href="/README_ru.md">Русский</a>.</strong></p>

---

## 🛠️ Techstack

- **Frontend:**
  - HTML5, CSS3
  - Vanilla JavaScript
- **Backend:**
  - Node.js
  - Express.js (REST API)
- **Database:**
  - Local JSON-based storage

---

## 🚀 Installation & Launch

Follow these steps to deploy the project on your local machine.

### Prerequisites

- Installed [Node.js](https://nodejs.org/) (version 14 or higher).

### Installation Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/y4lexzs/wirtschaftsquiz.git
   cd wirtschaftsquiz
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Environment setup:**
   Open `assets/js/storage.js` and ensure `API_URL` points to your server (default for local development is `http://localhost:3000/api`).

   ```javascript
   // assets/js/storage.js
   const API_URL = "http://localhost:3000/api";
   ```

4. **Start the server:**

   ```bash
   npm start
   ```

   The server will start on port `3000`.

5. **Open the application:**
   Navigate to `http://localhost:3000` in your browser.

---

## 📖 User Guide

1. **Getting Started:**

   - Open the application and register via the `auth.html` form.
   - After logging in, you will be taken to `index.html` or `dashboard.html`.

2. **Content Creation:**

   - Go to **Fragensammlung** (`question-bank.html`) and create some topics and questions.
   - Use the **Neues Quiz** in **Dashboard** (`dashboard.html`) to combine questions into a full quiz.

3. **Taking Tests:**

   - Share the quiz code or link with participants.
   - Participants take the test on the `take-quiz.html` page.
   - Results are available immediately after completion on the `review.html` page.

---

## ✨ Key Features

### 🔐 Users & Authentication

- **Registration & Login:** Simple user registration and authorization system.
- **Personalization:** Each user (teacher or student) has their own profile.
- **Security:** User data is stored in a built-in JSON database.

### 📚 Content

- **Topics:** Create and manage various topics.
- **Question Bank:** Add, edit, and delete questions.
- **Question Types:** Ability to create various question types (true/false, multiple choice, text input).
- **Quizzes:** Create and manage quizzes.

### 📝 Quiz Editor

- **Builder:** Intuitive interface for assembling quizzes from created questions.
- **Flexibility:** Ability to select specific questions from the bank to include in the test.
- **Sharing:** Unique codes for quick sharing and access to quizzes.

### 🚀 Taking Quizzes & Analytics

- **Interactive Player:** Convenient interface for taking tests.
- **Instant Feedback:** Users see results immediately.
- **Review:** Detailed view of correct and incorrect answers after completion.

---

## 📂 Project Structure

```
IDPA_readme/
├── assets/                 # Static resources
│   ├── css/styles.css      # Styles
│   └── js/                 # App logic (API, UI controllers)
│       ├── storage.js      # API & Database interaction
│       └── ...             # Scripts for each page and more
├── data/                   # Data storage (auto-created)
│   └── db.json             # Main database (JSON)
├── node_modules/           # Project dependencies
├── auth.html               # Login/Registration page
├── dashboard.html          # Dashboard
├── index.html              # Home page
├── new-question.html       # Question creation page
├── question-bank.html      # Question bank
├── quiz-editor.html        # Quiz editor
├── review.html             # Results review page
├── server.js               # Backend server entry point
├── take-quiz.html          # Quiz player page
├── package.json            # Project manifest & scripts
├── LICENSE                 # License file
└── README.md               # Project documentation
```

---

## 🤝 Contribution

If you want to improve the project, please:

1. Fork the repository.
2. Create a branch for your feature (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

---

## 📄 License

This project is distributed under the MIT license. See the [LICENSE](LICENSE) file for details.

---

<p align="center">*Developed with ❤️ as part of the IDPA educational project.*</p>
