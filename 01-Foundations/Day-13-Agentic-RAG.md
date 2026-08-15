# Day 13 – Agentic RAG (Part 1)

## Learning Objective

Understand how Agentic RAG extends traditional Retrieval-Augmented Generation by adding reasoning, planning, decision-making, and iterative retrieval capabilities.

---

# What is Agentic RAG?

Agentic RAG combines:

- Retrieval-Augmented Generation (RAG)
- AI Agents
- Reasoning
- Decision Making
- Planning
- Iterative Search

Traditional RAG retrieves information and generates an answer.

Agentic RAG decides:

- What information is needed
- Where to retrieve it
- Whether retrieved information is sufficient
- If additional retrieval is required
- How to produce the best answer

---

# Traditional RAG vs Agentic RAG

## Traditional RAG

Flow:

User Query
→ Retrieve Documents
→ Generate Answer

Characteristics:

- Simple architecture
- Single retrieval step
- Fast execution
- Limited reasoning

---

## Agentic RAG

Flow:

User Query
→ Agent Reasoning
→ Retrieval Planning
→ Information Retrieval
→ Result Evaluation
→ Additional Retrieval (if required)
→ Final Answer

Characteristics:

- Multi-step reasoning
- Adaptive retrieval
- Better accuracy
- Dynamic decision making
- More enterprise-ready

---

# Core Components of Agentic RAG

## 1. Reasoning Engine

Responsible for:

- Understanding user intent
- Determining information requirements
- Creating retrieval strategy

Example:

User asks:

"Why did revenue decrease in Branch B?"

Agent decides:

- Retrieve revenue data
- Compare historical performance
- Analyze doctor contribution
- Review appointment trends

---

## 2. Retrieval Planner

Creates a retrieval plan.

Example:

Step 1:
Retrieve revenue data

Step 2:
Retrieve doctor-wise performance

Step 3:
Retrieve branch-wise trends

Step 4:
Combine findings

---

## 3. Retrieval System

Collects information from:

- Vector Databases
- SQL Databases
- APIs
- Documents
- Enterprise Systems

---

## 4. Evaluation Layer

Checks:

- Relevance
- Completeness
- Confidence

If information is insufficient:

Agent performs another retrieval cycle.

---

## 5. Response Generation

Produces the final answer using:

- Retrieved Context
- Agent Reasoning
- Business Logic

---

# Agentic RAG Workflow

User Query
→ Agent Reasoning
→ Retrieval Planning
→ Information Retrieval
→ Evaluate Results
→ Additional Retrieval (Optional)
→ Generate Final Answer

---

# Practical Example 1 – MoM Insight 360

Business Question:

Why is Branch B underperforming this month?

Agent Process:

1. Retrieve revenue data
2. Compare with previous months
3. Analyze doctor contribution
4. Analyze appointment conversion
5. Review referral performance
6. Generate findings

Result:

Executive-level business insights.

---

# Practical Example 2 – IntelliHire Resume Studio

Business Question:

Find the best Python Developer candidate.

Agent Process:

1. Retrieve job description
2. Extract required skills
3. Search resumes
4. Compare skills
5. Rank candidates
6. Generate recommendation

Result:

Smarter hiring decisions.

---

# Benefits of Agentic RAG

- Better retrieval accuracy
- Multi-step reasoning
- Dynamic decision making
- Reduced hallucinations
- Improved enterprise adoption
- More intelligent AI systems

---

# Key Takeaway

Traditional RAG retrieves information.

Agentic RAG thinks, decides, retrieves, evaluates, and learns.

This makes AI systems more intelligent and capable of solving real-world business problems.

---

# Day 13 Part 1 Summary

Learned:

- Agentic RAG Fundamentals
- Traditional RAG vs Agentic RAG
- Agent Reasoning
- Retrieval Planning
- Evaluation Layer
- Iterative Retrieval
- Enterprise Use Cases

Next:

Day 13 Part 2

- Agentic Workflows
- Planning Strategies
- Reflection Loops
- Multi-Step Retrieval
- Advanced Agentic RAG Patterns

Day 13 — Part 2
Agentic RAG Implementation Patterns
Learning Objective

Understand how AI agents:

Plan retrieval strategies
Decide when retrieval is required
Break complex tasks into smaller tasks
Use tools intelligently
Reflect on their answers
Self-correct mistakes
Improve answer quality through iterative reasoning
1. Retrieval Planning

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
Analyze
   ↓
Retrieve Again
   ↓
Answer

The agent first decides:

What information is needed?
Where can I find it?
Which tool should I use?
Example

User asks:

Which branch generated the highest revenue last quarter?

Agent plan:

Step 1: Find branch revenue data
Step 2: Compare branches
Step 3: Validate results
Step 4: Generate answer
2. Query Decomposition

Complex questions are split into smaller questions.

User Query
Why did JP Nagar revenue decrease while
Sahakar Nagar increased?

Agent creates:

Q1 Revenue of JP Nagar?
Q2 Revenue of Sahakar Nagar?
Q3 Appointment count?
Q4 Doctor referrals?
Q5 Final comparison?

This improves retrieval quality.

3. Multi-Step Retrieval

Instead of one search:

Search Once
Answer

Agentic RAG performs:

Retrieve
Analyze
Retrieve Again
Validate
Answer
MoM Insight 360 Example

Executive asks:

Why is revenue down?

Agent:

Retrieve revenue
Retrieve scans
Retrieve doctors
Retrieve appointments
Analyze relationships
Generate explanation
4. Reflection Loop

After generating an answer:

Agent asks itself:

Is this answer complete?

Do I need more information?

Should I verify this result?

This is called Reflection.

5. Self-Correction

Agent discovers an issue:

Answer confidence low

Then:

Retrieve more data
Validate again
Improve answer

Process:

Think
Review
Correct
Answer
6. Tool-Augmented Retrieval

Modern agents can use multiple tools.

Examples:

Databases
SQL Server
PostgreSQL
MySQL
APIs
Weather API
Finance API
CRM API
Documents
PDF
Word
Excel
Search
Enterprise Search
Vector Database
Web Search
7. Enterprise Example – MoM Insight 360

Question:

Which branch missed its target and why?

Agent workflow:

Get target
Get actual revenue
Calculate gap
Analyze appointments
Analyze doctor referrals
Identify causes
Generate report
8. Enterprise Example – IntelliHire Resume Studio

Recruiter asks:

Find the best Python developer.

Agent:

Retrieve resumes
Extract skills
Compare JD
Rank candidates
Generate report
9. Key Difference
Traditional RAG
Retrieve → Answer
Agentic RAG
Plan
Reason
Retrieve
Validate
Reflect
Correct
Answer
Part 2 Key Takeaway

Agentic RAG is not just retrieval. It adds planning, reasoning, validation, reflection, and self-correction to make AI systems more intelligent and reliable.