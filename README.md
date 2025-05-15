
# AI-Powered Code Review System

This project is a full-stack AI Code Review system that leverages large language models to provide automatic feedback on source code. It includes:

- **frontend** built with Vite + React
- **backend** built using Node.js + Express
- Integration with external AI APIs (e.g., Gemini)
- Local database setup (MongoDB)

---

## GitHub Repository

> **GitHub Repository URL:** 

---

## Project Structure

```
CODE-REVIEW/
├── Frontend/               # Frontend React application
│   ├── index.html
│   ├── vite.config.js
│   ├── package.json
│   ├── src/
├── server.js               # Backend main entry
├── package.json            # Backend dependencies
├── .env.example            # Example environment configuration
```

---

## Installation Instructions

### Prerequisites

- Node.js
- npm or yarn
- MongoDB installed locally or via Atlas

---

### 1. Clone the Repository

```bash
git clone <your-repo-link>
cd CODE-REVIEW
```

---

### 2. Backend Setup

```bash
npm install
```

Create a `.env` file in the root directory:

```bash
cp .env.example .env
```

Edit `.env` and add your keys:

```
GOOGLE_GEMINI_KEY=your_google_key
MONGODB_URI=mongodb://localhost:27017/ai-code-review
PORT=5001
```

Start backend server:

```bash
node server.js
```

---

### 3. Frontend Setup

```bash
cd Frontend
npm install
npm run dev
```

Frontend will be available at: [http://localhost:5173](http://localhost:5173)

---

## Requirements

### Backend (`package.json`)

```json
{
  "dependencies": {
    "axios": "^1.6.0",
    "cors": "^2.8.5",
    "dotenv": "^16.0.3",
    "express": "^4.18.2",
    "openai": "^4.30.0"
  }
}
```

### Frontend (`Frontend/package.json`)

```json
{
  "dependencies": {
    "axios": "^1.6.0",
    "prismjs": "^1.29.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-simple-code-editor": "^0.11.0",
    "react-markdown": "^8.0.7",
    "rehype-highlight": "^6.0.0"
  },
  "devDependencies": {
    "vite": "^6.3.5"
  }
}
```

---

## Shell Scripts / Commands

- Start backend: `node server.js`
- Start frontend: `cd Frontend && npm run dev`

---

## Notes

- MongoDB is required for logging and evaluation data.
- Replace all placeholder API keys with valid ones in your `.env`.
- Use `npm install` or `yarn` in both root and `/Frontend` folders.


