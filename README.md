# 🥊 AI Battle Arena

AI Battle Arena is a platform where multiple AI models compete to solve the same problem, and an AI Judge evaluates their responses to determine the best answer.

The goal is to help users compare AI-generated solutions and identify the most accurate, complete, and helpful response.

---

## 🚀 Features

- Submit a single prompt to multiple AI models
- Generate responses from different LLMs
- AI Judge evaluates each response
- Automatic scoring system
- Winner selection based on scores
- Side-by-side solution comparison
- Modular architecture using LangGraph

---

## 🏗️ Architecture

```text
┌─────────────┐
│    USER     │
└──────┬──────┘
       │
       │ Problem
       ▼
┌──────────────────────┐
│   LangGraph Flow     │
└──────────┬───────────┘
           │
     ┌─────┴─────┐
     │           │
     ▼           ▼
┌─────────┐ ┌─────────┐
│ Mistral │ │ Gemini  │
└────┬────┘ └────┬────┘
     │           │
     ▼           ▼
 Solution 1   Solution 2
      \         /
       \       /
        ▼     ▼
   ┌─────────────┐
   │  AI Judge   │
   └──────┬──────┘
          │
          ▼
 ┌─────────────────┐
 │ Score Solution1 │
 │ Score Solution2 │
 │ Select Winner   │
 └────────┬────────┘
          │
          ▼
        USER
```

---

## ⚙️ Workflow

### Step 1
User submits a problem or question.

### Step 2
LangGraph orchestrates the complete execution flow.

### Step 3
Mistral generates the first solution.

### Step 4
Gemini generates the second solution.

### Step 5
Both solutions are sent to the AI Judge.

### Step 6
The AI Judge evaluates responses based on:

- Accuracy
- Relevance
- Clarity
- Completeness
- Reasoning Quality

### Step 7
Scores are assigned.

### Step 8
Final results are displayed to the user.

---

## 🛠️ Tech Stack

### Frontend

- React.js
- TypeScript
- Tailwind CSS

### Backend

- Node.js
- Express.js
- TypeScript

### AI Orchestration

- LangGraph
- LangChain

### AI Models

- Gemini
- Mistral
- Cohere (Planned)

---

## 📂 Project Structure

```bash
AI-Battle-Arena/
│
├── frontend/
│   ├── src/
│   ├── components/
│   ├── pages/
│   └── services/
│
├── backend/
│   ├── src/
│   │   ├── graph/
│   │   ├── models/
│   │   ├── judge/
│   │   ├── routes/
│   │   └── controllers/
│   │
│   └── server.ts
│
├── .env
├── package.json
└── README.md
```

---

## 🔑 Environment Variables

Create a `.env` file in the root directory.

```env
GEMINI_API_KEY=your_gemini_api_key

MISTRAL_API_KEY=your_mistral_api_key

COHERE_API_KEY=your_cohere_api_key
```

---

## 📦 Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/ai-battle-arena.git
```

### Move into Project

```bash
cd ai-battle-arena
```

### Install Dependencies

```bash
npm install
```

### Start Development Server

```bash
npm run dev
```

---

## 🎯 Example

### User Prompt

```text
Explain the difference between TCP and UDP.
```

### Mistral Response

```text
TCP is connection-oriented...
```

### Gemini Response

```text
TCP establishes a connection before data transfer...
```

### AI Judge Output

```text
Mistral Score: 8.5/10

Gemini Score: 9.2/10

Winner: Gemini
```

---

## 🔮 Future Improvements

- Add GPT models
- Add Claude integration
- Real-time battle visualization
- Battle history
- User voting system
- AI leaderboard
- Export battle reports
- Multi-round tournaments

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Open a Pull Request

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Ajay Gour**

B.Tech Student | MERN Developer | AI Enthusiast

Building projects to learn, experiment, and explore modern AI systems.
