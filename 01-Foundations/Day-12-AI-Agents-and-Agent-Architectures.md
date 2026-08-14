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

Day 12 – AI Agents & Agent Architectures
Part 2 – Advanced Agent Architectures
Learning Objective

Understand how modern AI systems use multiple agents, memory, tools, planning, and reflection to solve complex business problems.

Why Agent Architectures Matter

Traditional AI systems answer questions.

Agent-based AI systems can:

Plan tasks
Use tools
Make decisions
Collaborate with other agents
Learn from feedback
Execute multi-step workflows

This makes them suitable for enterprise applications.

Single Agent Architecture

A single agent handles the complete workflow.

Flow
User Request
      ↓
   Agent
      ↓
 Tool Usage
      ↓
 Response
Advantages
Easy to build
Lower cost
Faster implementation
Suitable for simple tasks
Limitations
Difficult to scale
Limited specialization
Complex workflows become difficult
Example

Resume screening assistant

User uploads resume

↓

Agent reads resume

↓

Compares with job description

↓

Returns match score

Multi-Agent Architecture

Multiple agents collaborate to solve a problem.

Flow
User Request
       ↓
Coordinator Agent
       ↓
 ┌─────────────┬─────────────┬─────────────┐
 ↓             ↓             ↓
Research     Analysis     Planning
 Agent        Agent        Agent
       ↓
Reporting Agent
       ↓
Final Response
Advantages
Better scalability
Improved accuracy
Specialized expertise
Easier maintenance
Example

Business Intelligence Platform

Research Agent → Collect KPIs

Analysis Agent → Analyze trends

Forecast Agent → Predict growth

Reporting Agent → Generate insights

Tool-Using Agents

Agents become powerful when they can access external tools.

Examples:

Databases
SQL Server
PostgreSQL
MySQL
APIs
Weather APIs
Payment APIs
CRM APIs
Search
Enterprise search
Internet search
Documents
PDF
Word
Excel
Analytics
Power BI
Tableau
Python
Planning Agents

Planning agents break large goals into smaller tasks.

Example

Goal:

Create Monthly Revenue Report

Plan

Step 1 → Retrieve Revenue Data

Step 2 → Clean Data

Step 3 → Analyze Trends

Step 4 → Generate Charts

Step 5 → Create Executive Summary

Step 6 → Deliver Report

This improves reliability and task completion.

Reflection Agents

Reflection is the ability of an AI agent to review its own work.

Process
Think
   ↓
Act
   ↓
Review
   ↓
Improve

Benefits:

Better quality responses
Reduced errors
Continuous improvement
Memory Systems

Modern agents use memory to improve performance.

Short-Term Memory

Current conversation context

Long-Term Memory

Historical interactions

Knowledge Memory

External knowledge sources

Examples:

Vector databases
Knowledge bases
Company documents
Agent Frameworks
LangGraph

Features:

Stateful workflows
Multi-agent orchestration
Human-in-the-loop support

Use Cases:

Enterprise AI
Complex workflows
CrewAI

Features:

Role-based agents
Agent collaboration

Use Cases:

Research teams
Business workflows
AutoGen

Features:

Agent-to-agent communication
Collaborative problem solving

Use Cases:

Automation
AI team simulations
Real-World Application – MoM Insight 360

Possible Agents:

KPI Agent

Retrieve KPIs

Revenue Agent

Analyze revenue trends

Forecast Agent

Predict future growth

Executive Agent

Generate business insights

Real-World Application – IntelliHire Resume Studio

Possible Agents:

Resume Agent

Read resumes

JD Matching Agent

Compare job descriptions

Ranking Agent

Rank candidates

Reporting Agent

Generate hiring reports

Future of AI Agents

Emerging Trends:

Autonomous Agents
Multi-Agent Teams
Agentic RAG
Self-Improving Agents
Enterprise AI Assistants
AI Workforce Collaboration
Key Takeaway

AI is evolving beyond chatbots.

The future belongs to intelligent agents that can:

Reason
Plan
Use tools
Collaborate
Learn
Execute tasks

A single AI assistant is powerful.

A coordinated team of AI agents is transformational.

Agent Frameworks Cheat Sheet
1. LangGraph
What is it?

LangGraph is a framework built on LangChain that helps create stateful AI agent workflows using graph-based execution.

Key Features
Stateful workflows
Multi-agent orchestration
Human-in-the-loop support
Complex decision trees
Memory integration
Best For

✅ Enterprise AI Applications
✅ Long-running workflows
✅ Agentic RAG Systems
✅ Multi-step reasoning

Example
User Query
    ↓
Research Agent
    ↓
Analysis Agent
    ↓
Reporting Agent
    ↓
Final Response
Learning Note

Think of LangGraph as:

"Workflow Engine for AI Agents"

2. CrewAI
What is it?

CrewAI allows multiple AI agents to work together as a team, where each agent has a specific role and responsibility.

Key Features
Role-based agents
Agent collaboration
Task delegation
Sequential workflows
Team-based execution
Best For

✅ Research Teams
✅ Business Process Automation
✅ Recruitment Systems
✅ Analytics Projects

Example
Manager Agent
      ↓
 ┌────┴────┐
 ↓         ↓
Research  Analysis
 Agent     Agent
      ↓
Report Agent
      ↓
Final Output
Learning Note

Think of CrewAI as:

"AI Employees Working as a Team"

3. AutoGen
What is it?

AutoGen is a Microsoft framework that enables agents to communicate and collaborate automatically.

Key Features
Agent-to-agent communication
Collaborative problem solving
Conversation-based workflows
Human-agent collaboration
Best For

✅ Software Development Agents
✅ Research Automation
✅ Complex Decision Making

Example
Developer Agent
       ↔
Reviewer Agent
       ↔
Testing Agent
       ↓
Final Solution
Learning Note

Think of AutoGen as:

"Agents Talking to Each Other"

4. OpenAI Agents SDK
What is it?

A framework for building AI agents using OpenAI models with tools, memory, handoffs, and workflows.

Key Features
Tool calling
Agent handoffs
Multi-agent systems
Memory support
Workflow orchestration
Best For

✅ Production Applications
✅ AI Assistants
✅ Enterprise Automation

Learning Note

Think of OpenAI Agents SDK as:

"Production-Ready AI Agent Framework"

Framework Comparison
Framework	Main Focus	Best For
LangGraph	Workflow Orchestration	Complex Enterprise Workflows
CrewAI	Team-Based Agents	Multi-Agent Collaboration
AutoGen	Agent Communication	Collaborative Problem Solving
OpenAI Agents SDK	Production Agents	Enterprise Applications
Easy Memory Trick
LangGraph  → Workflow
CrewAI     → Teamwork
AutoGen    → Communication
OpenAI SDK → Production
My Personal Understanding
LangGraph
   ↓
Build Agent Workflows

CrewAI
   ↓
Build Agent Teams

AutoGen
   ↓
Enable Agent Conversations

OpenAI Agents SDK
   ↓
Deploy Production Agents