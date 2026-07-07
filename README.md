# Quiz CLI

![License](https://img.shields.io/badge/license-MIT-blue)
![Version](https://img.shields.io/badge/version-1.0.0-orange)
![Node](https://img.shields.io/badge/node-%3E%3D18.0.0-339933)

## 📖 Project Overview

**Quiz CLI** is an interactive command-line quiz game for learning JavaScript and general programming concepts.

It presents multiple-choice questions in a terminal UI, lets users choose a category, select how many questions to answer, and shows a score summary with explanations for incorrect answers.

### Key features
- Category-based quiz selection
- Optional question count selection
- Randomized question order
- Instant feedback after each answer
- Final score and review of missed questions
- Colorized terminal output using ANSI escape codes

### Target audience
- Beginners learning JavaScript and Node.js
- Developers who want a quick terminal-based knowledge check
- Educators or students looking for a lightweight quiz game

## 🛠️ Tech Stack & Tools

- **Runtime:** Node.js `>=18.0.0`
- **Module system:** ES Modules (`"type": "module"`)
- **Core Node APIs used:**
  - `node:fs/promises`
  - `node:url`
  - `node:path`
  - `node:readline`
- **UI:** Terminal / command-line interface
- **Data format:** JSON (`data/questions.json`)
- **Testing:** Node.js built-in test runner (`node --test`)
- **License:** MIT

## 📁 File Structure

```text
quiz-cli/
├── data/
│   └── questions.json      # Quiz categories, questions, answers, and explanations
├── src/
│   ├── colors.js           # ANSI color helpers for terminal output
│   ├── input.js            # Readline helpers for prompts and selections
│   └── quiz.js             # Quiz class, scoring, progress, and results logic
├── index.js                # Application entry point
├── package.json            # Project metadata and npm scripts
└── README.md               # Project documentation
```

### Key files
- **`index.js`**: Main entry point that loads questions and runs the game loop
- **`src/quiz.js`**: Implements quiz flow, scoring, progress display, and result summary
- **`src/input.js`**: Handles user input via Node.js readline
- **`src/colors.js`**: Adds terminal colors and formatting
- **`data/questions.json`**: Stores all quiz content
- **`package.json`**: Defines scripts, Node version requirement, and license

## ⚙️ Setup Instructions

### Prerequisites
- Node.js **18.0.0 or newer**
- npm (bundled with Node.js)

### Installation

1. Clone the repository.
   ```bash
   git clone <repository-url>
   cd test-app
   ```

2. Install dependencies.
   ```bash
   npm install
   ```

3. Start the quiz.
   ```bash
   npm start
   ```

### Environment variables

No environment variables are required for this project.

### Docker

No Dockerfile or `docker-compose.yml` was found in the repository.

## 🚀 Usage Examples

### Run the application

```bash
npm start
```

This launches the interactive quiz in your terminal.

### How the quiz works

1. Choose a category.
2. Choose how many questions to answer.
3. Enter the number corresponding to your answer.
4. Review your score and explanations at the end.
5. Choose whether to play again.

### Run tests

```bash
npm test
```

The repository defines a Node.js test script (`node --test`), but no test files were found in the current codebase.

### Production build

No build step is configured for this project.

## 📡 API Reference

This project does not expose an HTTP API.

### Public interfaces

- `Quiz` class in `src/quiz.js`
- Input helpers in `src/input.js`
- Color helpers in `src/colors.js`

## 🔄 CI/CD Pipeline

No CI/CD workflows were found in `.github/workflows/`.

## 🤝 Contributing

Contributions are welcome.

Suggested workflow:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run `npm start` to verify the quiz still works
5. Run `npm test` if tests are added
6. Open a pull request

### Contribution notes
- Keep quiz content clear and accurate
- Preserve the terminal-friendly user experience
- Follow the existing ES Module style

## 📄 License

This project is licensed under the **MIT License**.

The license is declared in `package.json`. A separate `LICENSE` file was not found in the repository.
