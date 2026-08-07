# Day 09 – AI Agents & Tool Calling Fundamentals

## Introduction

Large Language Models (LLMs) are powerful at generating text, but they have limitations.

They cannot:

- Access real-time information by themselves
- Query databases directly
- Read local files automatically
- Execute code
- Call APIs
- Perform actions in external systems

This is where AI Agents come in.

AI Agents extend LLM capabilities by allowing them to interact with tools, systems, and external data sources.

---

# What is an AI Agent?

An AI Agent is an AI system that can:

1. Understand a goal
2. Plan actions
3. Use tools when needed
4. Observe results
5. Decide next steps
6. Deliver the final outcome

Simple Formula:

AI Agent = LLM + Reasoning + Tools + Memory + Actions

---

# Traditional AI vs AI Agent

## Traditional LLM

User Question
↓
LLM
↓
Answer

The model can only use its training knowledge.

---

## AI Agent

User Goal
↓
LLM
↓
Reasoning
↓
Tool Selection
↓
Execute Tool
↓
Observe Result
↓
Generate Final Answer

The agent can interact with the outside world.

---

# What is Tool Calling?

Tool Calling is the ability of an AI model to invoke external tools to complete a task.

Examples:

- Search the web
- Query databases
- Read PDFs
- Execute Python code
- Send emails
- Call APIs
- Create reports

Instead of guessing, the AI retrieves actual information.

---

# Why Tool Calling Matters

Without Tools:

"What is today's USD exchange rate?"

AI may provide outdated information.

With Tools:

AI calls a currency API and returns live data.

Result:

More accurate answers.

---

# Agent Workflow

Step 1:
Receive Goal

Example:
"Find the best-performing branch last month."

Step 2:
Reason

Determine what information is required.

Step 3:
Select Tool

Choose database query tool.

Step 4:
Execute Tool

Retrieve branch performance data.

Step 5:
Analyze Results

Compare performance metrics.

Step 6:
Generate Answer

Provide the final recommendation.

---

# Core Components of AI Agents

## 1. LLM Brain

Responsible for:

- Understanding requests
- Reasoning
- Planning

Examples:

- GPT
- Claude
- Gemini

---

## 2. Memory

Stores information across steps.

Types:

### Short-Term Memory

Current conversation.

### Long-Term Memory

Past interactions and knowledge.

---

## 3. Tools

External capabilities.

Examples:

- Search Tool
- Database Tool
- Python Tool
- API Tool
- File Tool

---

## 4. Planning

Agent determines:

- What should happen first?
- What information is missing?
- Which tool should be used?

---

## 5. Action Layer

Executes tasks.

Examples:

- Create report
- Query database
- Generate chart

---

# Single-Agent Architecture

User
↓
Agent
↓
Tools
↓
Answer

Useful for:

- Personal assistants
- Chatbots
- Small automation systems

---

# Multi-Agent Architecture

User
↓
Coordinator Agent

├── Research Agent
├── Data Agent
├── Reporting Agent
└── Validation Agent

↓

Final Answer

Useful for:

- Enterprise AI Systems
- Complex workflows
- Large-scale automation

---

# Real Example – MoM Insight 360

Management asks:

"Which branch missed budget targets and why?"

Agent Workflow:

Step 1:
Retrieve Budget Data

Step 2:
Retrieve Actual Revenue

Step 3:
Calculate Variance

Step 4:
Identify Root Cause

Step 5:
Generate Insights

Step 6:
Provide Recommendations

Tools Used:

- SQL Database
- KPI Engine
- Reporting Layer

---

# Real Example – IntelliHire Resume Intelligence Studio

Recruiter asks:

"Find the best Python Developer candidate."

Agent Workflow:

Step 1:
Read Job Description

Step 2:
Retrieve Candidate Profiles

Step 3:
Compare Skills

Step 4:
Calculate Match Scores

Step 5:
Rank Candidates

Step 6:
Generate Hiring Recommendation

Tools Used:

- Resume Database
- Embedding Search
- Matching Engine

---

# Popular Agent Frameworks

## LangChain

Provides tool calling and agent orchestration.

## LangGraph

State-based agent workflows.

## CrewAI

Multi-agent collaboration framework.

## AutoGen

Agent-to-agent communication.

## OpenAI Agents SDK

Modern framework for building AI agents.

---

# Key Takeaways

- AI Agents extend LLM capabilities.
- Tool Calling enables interaction with external systems.
- Agents can reason, plan, act, and observe.
- Tool Calling reduces hallucinations.
- Enterprise AI relies heavily on Agent + Tool architectures.
- Future AI applications will increasingly be Agent-based.

---

# Summary

AI Agents transform AI from a conversational assistant into an active problem-solving system.

Traditional AI answers questions.

AI Agents complete tasks.

Tool Calling is the bridge that connects AI with real-world systems, databases, APIs, and business workflows.