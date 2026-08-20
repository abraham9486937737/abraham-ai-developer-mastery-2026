# Day 16 – Agent Planning, Reasoning & Decision Making

## Part 1 – Agent Planning Fundamentals

### 🎯 Learning Objectives

By the end of Part 1, you will understand:

- What planning means in AI agents
- Why planning is important
- Goal decomposition
- Task planning
- Sequential planning
- Hierarchical planning
- Dynamic planning
- Planning in Agentic RAG
- Enterprise planning workflows
- How modern AI agents create execution plans

---

## 🧠 1. What is Planning?

Planning is the process of deciding what actions should be performed to achieve a goal.

Traditional software follows predefined instructions.

Example:

Input
↓
Logic
↓
Output

AI Agents work differently.

Goal
↓
Plan
↓
Execute
↓
Observe
↓
Adjust
↓
Result

An AI Agent first decides:

- What needs to be done
- Which tools are required
- What information is needed
- What order tasks should follow

before execution begins.

---

## 🧠 2. Why Planning Matters

Without planning:

❌ Random actions

❌ Wrong tool selection

❌ Higher costs

❌ Inefficient workflows

❌ Poor decisions

❌ Unreliable results

With planning:

✅ Structured execution

✅ Better decisions

✅ Faster completion

✅ Reduced cost

✅ Improved accuracy

✅ Better user experience

Planning allows agents to work intelligently rather than react blindly.

---

## 🧠 3. Goal-Based Execution

AI Agents operate using goals.

Example:

User Request:

"Generate a monthly business report."

The agent does not immediately generate the report.

Instead it creates a goal:

Goal:
Generate a complete business performance report.

The goal then gets converted into smaller tasks.

This approach is called Goal-Based Execution.

---

## 🧠 4. Goal Decomposition

Large goals are broken into smaller manageable tasks.

Example:

Goal:
Analyze Hospital Performance

Agent Plan:

Step 1 → Collect Revenue Data

Step 2 → Collect Scan Counts

Step 3 → Calculate KPIs

Step 4 → Analyze Trends

Step 5 → Forecast Growth

Step 6 → Generate Report

This process is called Goal Decomposition.

Benefits:

✅ Easier execution

✅ Better accuracy

✅ Improved monitoring

✅ Better coordination

---

## 🧠 5. Task Planning

Task planning determines the order of execution.

Example:

User:
Analyze Branch Performance

Planner Agent:

Task 1 → Retrieve Revenue Data

Task 2 → Retrieve Budget Data

Task 3 → Compare Actual vs Budget

Task 4 → Analyze Revenue Gap

Task 5 → Generate Recommendations

The planner agent acts like a project manager.

---

## 🧠 6. Sequential Planning

Tasks execute one after another.

Example:

Task A
↓
Task B
↓
Task C
↓
Task D

Enterprise Example:

IntelliHire Resume Studio

Parse Resume
↓
Extract Skills
↓
Match Job Description
↓
Rank Candidate
↓
Generate Recommendation

Sequential planning is simple and predictable.

---

## 🧠 7. Hierarchical Planning

Complex goals require multiple levels of planning.

Main Goal
│
├── Revenue Analysis
├── KPI Analysis
├── Forecast Analysis
├── Doctor Analysis
└── Branch Analysis

Enterprise Example:

MoM Insight 360

Main Goal:
Executive Performance Dashboard

Sub Goals:

- Revenue Performance
- KPI Monitoring
- Budget Tracking
- Forecasting
- Branch Comparison

Hierarchical planning is commonly used in enterprise AI systems.

---

## 🧠 8. Dynamic Planning

Dynamic planning allows agents to change plans during execution.

Example:

Original Plan:

Retrieve Revenue Data
↓
Analyze Revenue

Problem:

Revenue database unavailable

Agent decides:

Retrieve Backup Data
↓
Continue Analysis

This ability to adapt makes AI Agents more powerful than traditional workflows.

Benefits:

✅ Flexibility

✅ Resilience

✅ Better fault tolerance

✅ Higher success rate

---

## 🧠 9. Planning vs Traditional Programming

Traditional Programming

Developer defines every step.

Example:

IF condition
THEN execute task

Everything is fixed.

AI Agent Planning

Developer defines the goal.

Agent decides:

- What to do
- When to do it
- Which tools to use
- How to reach the goal

Traditional Systems:
Rule-Based

AI Agents:
Goal-Based

---

## 🧠 10. Planning in Agentic RAG

Traditional RAG

Question
↓
Retrieve
↓
Answer

Agentic RAG

Question
↓
Plan Retrieval Strategy
↓
Select Sources
↓
Retrieve Information
↓
Validate Results
↓
Reason
↓
Generate Answer

Planning significantly improves retrieval quality.

Benefits:

✅ Better information selection

✅ Reduced hallucinations

✅ Improved reasoning

✅ More accurate responses

---

## 🏢 11. Enterprise Example – MoM Insight 360

User Request:

"Why did JP Nagar miss its monthly target?"

Planner Agent creates:

Step 1 → Retrieve Revenue Data

Step 2 → Compare Budget vs Actual

Step 3 → Analyze Scan Volume

Step 4 → Calculate ASK Rate

Step 5 → Forecast Impact

Step 6 → Generate Recommendations

Result:

Detailed business insight instead of a simple answer.

---

## 🎯 12. Enterprise Example – IntelliHire Resume Studio

User Request:

"Find the best Data Analyst candidate."

Planner Agent:

Analyze Job Description
↓
Identify Required Skills
↓
Evaluate Resumes
↓
Calculate Match Scores
↓
Rank Candidates
↓
Generate Recommendation

Result:

Smarter hiring decisions.

---

## 📚 Key Takeaways

✅ Planning determines how agents achieve goals

✅ Goal decomposition breaks large tasks into smaller tasks

✅ Task planning organizes execution steps

✅ Sequential planning executes tasks one by one

✅ Hierarchical planning manages complex goals

✅ Dynamic planning adapts to changing situations

✅ Agentic RAG uses planning before retrieval

✅ Planning transforms AI from reactive systems into intelligent problem solvers

---

## 💡 Key Learning

Memory helps agents remember.

Planning helps agents decide what to do next.

Reasoning helps agents decide the best action.

Together, Memory + Planning + Reasoning form the foundation of intelligent AI Agents.

Part 2 – Agent Reasoning & Decision Making
🎯 Learning Objectives

By the end of Part 2, you will understand:

What reasoning means in AI agents
Why reasoning is important
Chain of Thought (CoT)
Tree of Thoughts (ToT)
ReAct Framework
Reflection
Self-Correction
Decision Making
Reasoning in Agentic RAG
Enterprise reasoning workflows
🧠 1. What is Reasoning?

Reasoning is the process of thinking through a problem before taking action.

Traditional Software:

Input
↓
Rule
↓
Output

AI Agents:

Input
↓
Think
↓
Evaluate
↓
Choose Best Action
↓
Execute

Reasoning enables agents to solve problems rather than simply follow instructions.

🧠 2. Why Reasoning Matters

Without reasoning:

❌ Wrong conclusions

❌ Poor decisions

❌ Inefficient actions

❌ Hallucinations

❌ Inconsistent outputs

With reasoning:

✅ Better decisions

✅ Improved accuracy

✅ Logical problem solving

✅ Higher reliability

✅ Better user outcomes

🧠 3. Chain of Thought (CoT)

Chain of Thought means solving a problem step by step.

Example:

Question:

Revenue in June = ₹20 Lakhs
Revenue in July = ₹25 Lakhs


What is the growth percentage?

Agent Reasoning:

Step 1:
Difference = 25 - 20


Step 2:
Difference = 5


Step 3:
Growth % = (5/20) × 100


Step 4:
Growth % = 25%

Answer:

Revenue Growth = 25%

The agent explains how it arrived at the answer.

🧠 4. Tree of Thoughts (ToT)

Sometimes multiple solutions exist.

Instead of following one path, the agent explores several possibilities.

Example:

Question:

How can branch revenue be increased?

Branch A:

Increase Marketing

Branch B:

Increase Conversions

Branch C:

Improve Doctor Referrals

The agent evaluates all options and selects the best solution.

Benefits:

✅ Better decision quality

✅ Multiple solution exploration

✅ Reduced bias

🧠 5. ReAct Framework

ReAct stands for:

Reason + Act

Process:

Question
↓
Reason
↓
Take Action
↓
Observe Result
↓
Reason Again
↓
Final Answer

Example:

User:

Why is revenue decreasing?

Agent:

Reason:
Need revenue data


Action:
Query database


Observe:
Revenue dropped 15%


Reason:
Need scan count data


Action:
Retrieve scan statistics


Observe:
Scan volume decreased


Conclusion:
Lower scan volume caused revenue decline

This is one of the most important Agentic AI patterns.

🧠 6. Reflection

Reflection means reviewing previous work before finalizing a response.

Example:

Draft Answer
↓
Review Answer
↓
Identify Weaknesses
↓
Improve Answer
↓
Final Output

Human Equivalent:

Write
↓
Review
↓
Edit
↓
Publish

Benefits:

✅ Higher quality output

✅ Better reasoning

✅ Improved reliability

🧠 7. Self-Correction

Agents can detect and fix mistakes.

Example:

Calculation:

Revenue Growth = 15%

Validation Agent:

Check Calculation

Result:

Actual Growth = 25%

Agent:

Correct Error
↓
Update Answer

Benefits:

✅ Reduced errors

✅ Increased accuracy

✅ Better trustworthiness

🧠 8. Decision Making

Decision making is selecting the best action among alternatives.

Example:

Problem:

Revenue is declining

Possible Actions:

Option A:
Increase Marketing


Option B:
Improve Conversion Rate


Option C:
Increase Doctor Referrals

Agent evaluates:

Cost
Impact
Feasibility
Time

Then chooses the best action.

🧠 9. Reasoning Loop

Modern AI Agents operate using reasoning loops.

Observe
↓
Think
↓
Plan
↓
Act
↓
Evaluate
↓
Improve
↓
Repeat

This cycle continues until the goal is achieved.

🧠 10. Reasoning in Agentic RAG

Traditional RAG:

Question
↓
Retrieve
↓
Answer

Agentic RAG:

Question
↓
Plan
↓
Retrieve
↓
Reason
↓
Validate
↓
Reflect
↓
Answer

Reasoning makes retrieval more useful and accurate.

🏢 11. Enterprise Example – MoM Insight 360

User Question:

Why did revenue decline this month?

Agent Reasoning:

Step 1:
Analyze Revenue


Step 2:
Compare Previous Month


Step 3:
Analyze Scan Volume


Step 4:
Analyze ASK Rate


Step 5:
Evaluate Budget Impact


Step 6:
Generate Insight

Result:

Revenue declined because
scan volume dropped by 12%
while ASK rate remained stable.
🎯 12. Enterprise Example – IntelliHire Resume Studio

User Request:

Recommend the best candidate
for Data Analyst role.

Agent Reasoning:

Analyze JD
↓
Extract Skills
↓
Compare Candidates
↓
Calculate Match Scores
↓
Rank Candidates
↓
Validate Rankings
↓
Generate Recommendation

Result:

Candidate A selected
with 92% match score.
📚 Key Takeaways

✅ Reasoning helps agents think before acting

✅ Chain of Thought solves problems step-by-step

✅ Tree of Thoughts explores multiple solutions

✅ ReAct combines reasoning and actions

✅ Reflection improves answer quality

✅ Self-Correction reduces errors

✅ Decision Making selects the best action

✅ Agentic RAG becomes more powerful with reasoning

✅ Reasoning transforms AI from information retrieval into intelligent problem solving

💡 Key Learning

Memory remembers the past.

Planning decides what to do.

Reasoning decides the best way to do it.

Together:

Memory
+
Planning
+
Reasoning
=
Intelligent AI Agent
Frameworks to Research During Learning
LangGraph
Reasoning Strengths
Multi-Step Reasoning Workflows
State-Aware Decision Making
Reflection Loops
Checkpoint-Based Reasoning
Agentic RAG Support
Best For
Enterprise AI Systems
Complex Business Workflows
Multi-Agent Reasoning
CrewAI
Reasoning Strengths
Team-Based Decision Making
Role-Based Reasoning
Collaborative Problem Solving
Agent Delegation
Best For
Multi-Agent Collaboration
Business Process Automation
Team-Oriented AI Systems
AutoGen
Reasoning Strengths
Conversational Reasoning
Agent Discussions
Debate-Based Decisions
Autonomous Collaboration
Best For
Research Agents
Coding Agents
Autonomous AI Teams
Quick Comparison
Framework	Strength	Best Use Case
LangGraph	Workflow Reasoning	Enterprise AI Systems
CrewAI	Collaborative Reasoning	Multi-Agent Teams
AutoGen	Conversational Reasoning	Research & Coding Agents
Day 16 Final Understanding

Traditional Systems:

Rules
↓
Execution
↓
Result

Agentic Systems:

Memory
↓
Planning
↓
Reasoning
↓
Action
↓
Reflection
↓
Improvement

This is the foundation of modern Agentic AI. 🚀