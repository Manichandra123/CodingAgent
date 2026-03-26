# 🚀 AI Coding Agent

A production-style AI coding agent that can **plan, generate, execute, and fix code automatically** using LLMs and tool calling.

---

## 🧠 Overview

This project implements an AI agent that goes beyond simple prompting.  
It combines an LLM with tools and a structured execution loop to solve coding tasks end-to-end.

The agent follows a **ReAct-style workflow**:

User → LLM → Tool Call → Observation → LLM → Final Output

---

## ⚙️ Features

- 🧩 Task Planning (step-by-step execution)
- 💻 Code Generation (multi-language support)
- 📁 File Operations (create, read, update)
- ▶️ Code Execution (run and validate output)
- 🔁 Automatic Debugging (fix errors iteratively)
- 📊 Structured Outputs (JSON-based tool calls)

---

## 🛠️ Tools

The agent uses a custom tool layer:

- `write_file` → create or overwrite files  
- `read_file` → inspect existing code  
- `update_file` → modify and fix code  
- `run_code` → execute and validate code  

Each tool is designed with structured inputs and outputs to ensure reliable interaction with the LLM.

---

## 🧠 System Design

The agent is controlled using a structured system prompt that enforces:

- Planning before execution  
- Step-by-step tool usage  
- Output verification  
- Iterative error fixing  

This transforms the LLM from a text generator into a **problem-solving system**.

---

## 🔁 Agent Loop

The core logic is an execution loop that:

1. Sends user input to the LLM  
2. Parses structured JSON responses  
3. Executes tool calls  
4. Feeds results back as observations  

This enables continuous reasoning and improvement.


 
