# Day 12 – AI Agents & Agent Architectures

## Part 1 – AI Agents & Agent Architectures

### Learning Objective

Understand what an AI Agent is, how it is different from a traditional LLM or chatbot, and how agents use reasoning, planning, memory, tools, actions, and feedback to accomplish goals.

---

## 1. What is an AI Agent?

An AI Agent is a goal-oriented AI system that can understand a task, reason about it, create a plan, use tools, perform actions, observe results, and continue working toward the desired outcome.

A simple chatbot mainly responds to a user.

An AI Agent can work toward completing a task.

### Simple Difference

Traditional AI:

User Question → AI Answer

AI Agent:

User Goal → Understand → Reason → Plan → Act → Observe → Continue → Complete Goal

---

## 2. LLM vs AI Agent

### LLM

An LLM mainly:

- Understands language
- Generates responses
- Summarizes information
- Answers questions
- Generates text or code

### AI Agent

An AI Agent can:

- Understand a goal
- Reason about the problem
- Create a plan
- Select tools
- Retrieve information
- Perform actions
- Remember useful information
- Observe results
- Adjust the next action
- Continue until the task is completed

### Key Realization

> LLMs generate answers.  
> AI Agents work toward goals.

---

## 3. Core Components of an AI Agent

A practical AI Agent can contain several important components.

### 1. Perception

The agent receives information from:

- User requests
- Documents
- APIs
- Databases
- Files
- External systems

### 2. Memory

Memory helps the agent maintain useful information across steps or interactions.

Examples:

- Previous conversation
- User preferences
- Previous actions
- Retrieved information
- Task state

### 3. Reasoning

The agent analyzes the current situation and determines what should happen next.

### 4. Planning

The agent breaks a larger goal into smaller actions.

Example:

Goal:

"Prepare a branch performance report."

Possible plan:

1. Retrieve branch data
2. Calculate KPIs
3. Compare actual vs target
4. Identify important changes
5. Generate insights
6. Prepare the report

### 5. Tools

Tools allow the agent to interact with the real world.

Examples:

- Database
- Search
- Calculator
- Python
- API
- File system
- Business applications

### 6. Action / Execution

The agent executes the selected action using the appropriate tool.

### 7. Feedback

The agent observes the result and decides whether another action is required.

---

## 4. Basic AI Agent Architecture

A simple agent architecture can be understood as:

User Request
↓
Perception
↓
Memory
↓
Reasoning
↓
Planning
↓
Decision
↓
Tool / Action
↓
Observation
↓
Feedback
↓
Next Action or Final Response

This creates an iterative agent loop.

---

## 5. The Agent Loop

The important idea is that an agent does not always follow only one fixed step.

It can:

1. Understand the goal
2. Decide what information is required
3. Select a tool
4. Perform an action
5. Observe the result
6. Reason about the result
7. Decide the next action
8. Continue until the goal is achieved

This makes agents different from simple question-answering systems.

---

## 6. Practical Example – Data Science Laptop

User:

"Find me the best laptop for Data Science under ₹60,000."

A simple AI response may provide a list of laptops.

An AI Agent could potentially:

1. Understand the budget and requirement
2. Search available products
3. Compare CPU, RAM, GPU and storage
4. Check availability
5. Rank the options
6. Recommend the best option
7. Continue with ordering or tracking if the required tools are available

The agent is not only answering.

It is working toward completing the user's goal.

---

## 7. Real-World Application – MoM Insight 360

An AI Agent could support executive decision-making.

Example:

User:

"Why did revenue decrease in the JP Nagar branch this month?"

The agent could:

1. Retrieve branch revenue data
2. Compare current and previous periods
3. Retrieve appointment and scan data
4. Analyze doctor contribution
5. Check PRO performance
6. Identify significant changes
7. Generate an executive explanation

Possible flow:

User Question
→ Retrieve Data
→ Analyze
→ Compare
→ Reason
→ Generate Insight

This connects AI Agents with the RAG and Advanced RAG concepts learned earlier.

---

## 8. Real-World Application – IntelliHire Resume Studio

An AI Agent could help with recruitment.

Example:

"Find the most suitable candidates for this Data Analyst position."

The agent could:

1. Read the job description
2. Retrieve candidate resumes
3. Compare skills
4. Check experience
5. Calculate or evaluate suitability
6. Rank candidates
7. Generate recommendations

This combines:

RAG + Reasoning + Tools + Planning + Actions

---

## 9. AI Agent vs Traditional Software

Traditional software generally follows predefined logic.

Example:

Input
→ Rule
→ Process
→ Output

An AI Agent can dynamically determine the next step.

Example:

Goal
→ Reason
→ Decide
→ Use Tool
→ Observe
→ Reason Again
→ Next Action

This makes agent systems more flexible for complex tasks.

---

## 10. My Key Realization

The most important concept I understood today is:

> AI is evolving from answering questions to performing tasks.

An LLM provides intelligence for language and reasoning.

An Agent adds:

- Goals
- Planning
- Tools
- Memory
- Actions
- Feedback

Together, these capabilities allow AI systems to move closer to completing real-world tasks.

---

## Part 1 Key Takeaway

> "An AI Agent is not simply a chatbot. It is a goal-oriented system that can reason, plan, use tools, take actions, observe results, and continue working toward a goal."

---

## Part 1 Status

✅ AI Agent fundamentals understood  
✅ LLM vs AI Agent understood  
✅ Agent architecture understood  
✅ Perception, Memory and Reasoning understood  
✅ Planning and Decision Making understood  
✅ Tools and Actions understood  
✅ Feedback and Agent Loop understood  
✅ MoM Insight 360 application understood  
✅ IntelliHire application understood  
✅ Part 1 Learning Completed

### Day 12 Overall Status

🟡 **IN PROGRESS**

### Next

**Day 12 – Part 2: Advanced Agent Architectures, Tool Calling, Agent Memory, Multi-Agent Systems, Agentic RAG and Enterprise Agent Design**