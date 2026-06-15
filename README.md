# 🎓 Unified Campus Intelligence Dashboard

An AI-powered campus assistant built using **Next.js, FastAPI, and Model Context Protocol (MCP)** to unify fragmented campus services into a single intelligent platform.

---

## 📌 Problem Statement

Campus information is often scattered across multiple independent systems such as library portals, cafeteria menus, event websites, academic portals, and attendance systems. Students must switch between different applications to access routine information.

This project addresses this challenge by providing a unified AI-powered dashboard capable of retrieving and aggregating information from multiple campus services through independent MCP servers.

---

# 🚀 Features

### 📊 Unified Dashboard

* Attendance overview
* Assignment deadlines
* Upcoming campus events
* Library availability
* Cafeteria menu
* Study room status
* Quick campus insights

---

### 🤖 AI Campus Assistant

The AI Assistant can answer natural language queries such as:

* What's for lunch today?
* What events are happening?
* Show my library books.
* Find campus resources.
* Answer academic-related questions.

The assistant intelligently routes requests to the appropriate MCP service.

---

### 📚 Library MCP

Provides:

* Book search
* Availability status
* Due date information
* Library resource management

---

### 🍽 Cafeteria MCP

Provides:

* Daily menu
* Meal availability
* Food recommendations

---

### 🎉 Events MCP

Provides:

* Upcoming campus events
* Event details
* Schedule information

---

### 🎓 Academics MCP

Provides:

* Academic policies
* Student resources
* Course-related information

---

# 🏗 Architecture

```
                    User
                      │
                      ▼
            AI Campus Assistant
                      │
                      ▼
             AI Orchestrator
                      │
      ┌───────────────┼───────────────┐
      │               │               │
      ▼               ▼               ▼
 Library MCP    Events MCP    Cafeteria MCP
      │
      ▼
 Academics MCP
```

Each MCP server operates independently and exposes its own API endpoints.

The AI assistant uses tool/function calling to dynamically select and query the appropriate service.

---

# 🛠 Tech Stack

## Frontend

* Next.js
* React
* TypeScript
* Tailwind CSS

## Backend

* Python
* FastAPI
* Model Context Protocol (MCP)

## AI

* OpenRouter
* LLM Function Calling
* Multi-tool AI Orchestration

---

# 📂 Project Structure

```
app/
components/
data/
public/

backend/
├── app/
│   └── ai/
├── mcp/
│   ├── library/
│   ├── events/
│   ├── cafeteria/
│   └── academics/
```

---

# ⚙️ Installation

## Clone the repository

```
git clone <repository-url>
cd Unified-Campus-Intelligence-Dashboard
```

---

## Frontend

```
npm install
npm run dev
```

Runs on:

```
http://localhost:3000
```

---

## Backend AI

```
cd backend
python -m uvicorn app.main:app --reload --port 8000
```

---

## Library MCP

```
cd backend/mcp/library
python -m uvicorn main:app --reload --port 8001
```

---

## Events MCP

```
cd backend/mcp/events
python -m uvicorn main:app --reload --port 8002
```

---

## Cafeteria MCP

```
cd backend/mcp/cafeteria
python -m uvicorn main:app --reload --port 8003
```

---

## Academics MCP

```
cd backend/mcp/academics
python -m uvicorn main:app --reload --port 8004
```

---

# 🔑 Environment Variables

Create:

```
backend/.env
```

Example:

```
OPENAI_API_KEY=YOUR_API_KEY
OPENAI_BASE_URL=https://openrouter.ai/api/v1
OPENAI_MODEL=openrouter/free
```

---

# 💡 Example AI Queries

```
What's for lunch today?

What events are happening?

Show my library books.

Find academic resources.

Search for available books.
```

---

# 🎯 Key Highlights

✅ Unified campus dashboard

✅ AI-powered assistant

✅ Independent MCP servers

✅ Multi-tool orchestration

✅ Natural language interaction

✅ Modular microservice architecture

✅ Real-time campus information retrieval

---

# 🔮 Future Enhancements

* Smart study room booking
* Attendance analytics
* Assignment management
* Cross-module reasoning
* Personalized recommendations
* Real-time campus notifications

---

# 🎥 Demonstration

The demonstration showcases:

* Dashboard overview
* Library search
* Cafeteria recommendations
* Campus events
* AI Assistant
* MCP architecture

---

# 👨‍💻 Author

**Shivansh Kanodiya**

B.Tech, Electrical Engineering

AI-powered Unified Campus Intelligence Dashboard

---

## ⭐ Project Vision

**One dashboard for everything on campus.**

This project demonstrates how AI and Model Context Protocol (MCP) can unify fragmented campus services into a single intelligent, scalable, and user-friendly platform that enhances the student experience.
