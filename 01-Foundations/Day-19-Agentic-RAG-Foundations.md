Day 19 – Agentic RAG (Retrieval Augmented Generation)
Part 1 – RAG Fundamentals
🎯 Learning Objectives

By the end of Part 1, you will understand:

What is RAG
Why Large Language Models Hallucinate
Limitations of Standalone LLMs
Knowledge Retrieval Fundamentals
Embeddings & Vector Search
Traditional RAG Architecture
Components of a RAG System
RAG Workflow
Enterprise Applications of RAG
Why RAG is a Game Changer for AI
🧠 1. The Problem with Standalone LLMs

Large Language Models are trained on historical data.

Examples:

GPT
Claude
Gemini
Llama

They learn patterns from training datasets.

However:

Limitations

❌ Knowledge becomes outdated

❌ Cannot access private company data

❌ Cannot access latest business reports

❌ May generate incorrect information

❌ Can hallucinate answers

Example

User:

What was MoM Insight 360 revenue yesterday?

A standalone LLM does not know.

Why?

Because that information was never part of its training data.

🧠 2. What is Hallucination?

Hallucination occurs when an AI model generates information that sounds correct but is actually false.

Example

User:

Who won the MoM Innovation Award 2027?

LLM:

Dr. Smith won the award.

The model may invent an answer because it does not know the truth.

Problems Caused by Hallucinations

❌ Wrong business decisions

❌ Loss of trust

❌ Compliance risks

❌ Financial impact

❌ Poor user experience

🧠 3. What is RAG?
Definition

RAG stands for:

Retrieval Augmented Generation

Instead of relying only on model memory:

Question
   ↓
Retrieve Information
   ↓
Provide Context
   ↓
Generate Answer

The model retrieves relevant information before answering.

Simple Formula
LLM
+
Knowledge Retrieval
=
RAG
Human Example

Imagine a manager asked:

What was last month's revenue?

Instead of guessing:

Open report
Check data
Verify information
Give answer

RAG works similarly.

🧠 4. Why RAG Matters

Without RAG:

User Question
      ↓
LLM
      ↓
Answer

Knowledge is limited.

With RAG:

User Question
      ↓
Knowledge Search
      ↓
Relevant Documents
      ↓
LLM
      ↓
Answer

Knowledge becomes dynamic.

Benefits

✅ More accurate answers

✅ Uses latest information

✅ Accesses enterprise data

✅ Reduces hallucinations

✅ Improves trust

🧠 5. Core Components of a RAG System

A RAG system contains five major components.

Component 1 – Data Source

Examples:

PDFs
Excel Files
Databases
Websites
SharePoint
Business Reports
Component 2 – Embedding Model

Converts text into vectors.

Example:

Revenue increased by 15%
      ↓
Vector Representation

Machines understand vectors better than raw text.

Component 3 – Vector Database

Stores embeddings.

Popular options:

ChromaDB
Pinecone
Weaviate
Qdrant
Milvus

Purpose:

Fast similarity search.

Component 4 – Retriever

Searches for relevant information.

Example:

User asks:

Show revenue trend.

Retriever finds:

Revenue reports
KPI documents
Dashboard summaries
Component 5 – LLM

Uses retrieved information to generate the final response.

🧠 6. What are Embeddings?

Embeddings convert text into numerical representations.

Example:

Sales Revenue

becomes

[0.24, 0.91, 0.12, ...]

These vectors capture meaning.

Similar Meanings Stay Close

Example:

Revenue Analysis
Revenue Trends
Financial Performance

These vectors are stored near each other.

Different Meanings Stay Far Apart

Example:

Revenue Analysis


vs


Football Match

Vectors are far apart.

🧠 7. What is Vector Search?

Traditional Search:

Search:
Revenue

Looks for exact keywords.

Vector Search:

Searches by meaning.

Example:

User asks:

Business growth performance

System can retrieve:

Revenue reports
KPI trends
Financial summaries

Even if exact words are different.

Benefits

✅ Semantic search

✅ Better retrieval

✅ Context awareness

✅ More relevant results

🧠 8. Traditional RAG Architecture
User Question
        │
        ▼
Embedding Model
        │
        ▼
Vector Database
        │
        ▼
Retriever
        │
        ▼
Relevant Documents
        │
        ▼
LLM
        │
        ▼
Final Answer
🧠 9. RAG Workflow
Step 1

User asks question

What is July revenue?
Step 2

Question converted into embedding

Step 3

Vector database searched

Step 4

Relevant documents retrieved

Step 5

Context sent to LLM

Step 6

LLM generates answer

Result

Accurate response based on actual data.

🏢 10. Enterprise Example – MoM Insight 360
Data Sources
Revenue Reports
Budget Data
KPI Metrics
Forecast Reports
Doctor Performance Data
RAG Flow
User:
Show branch revenue trend


       ↓


Retriever


       ↓


Revenue Reports


       ↓


LLM


       ↓


Executive Insight
Benefits

✅ Accurate analytics

✅ Real-time business insights

✅ Better decisions

🎯 11. Enterprise Example – IntelliHire Resume Studio
Data Sources
Candidate Resumes
Job Descriptions
Skill Libraries
Interview Feedback
Hiring History
RAG Flow
Recruiter Question
       ↓


Resume Retrieval
       ↓


Candidate Context
       ↓


LLM
       ↓


Recommendation
Benefits

✅ Better candidate matching

✅ Faster recruitment

✅ Improved recommendations

🧠 12. RAG vs Fine-Tuning
Feature	RAG	Fine-Tuning
Uses Latest Data	✅	❌
Easy Updates	✅	❌
Lower Cost	✅	❌
Enterprise Knowledge	✅	Limited
Retraining Required	❌	✅
Enterprise Preference

Most organizations choose:

✅ RAG First

Then

✅ Fine-Tuning if required

📚 Key Takeaways

✅ LLMs can hallucinate

✅ RAG reduces hallucinations

✅ RAG retrieves knowledge before answering

✅ Embeddings convert text into vectors

✅ Vector databases enable semantic search

✅ RAG combines retrieval and generation

✅ Enterprise AI heavily depends on RAG

✅ MoM Insight 360 can use RAG for business intelligence

✅ IntelliHire Resume Studio can use RAG for recruitment intelligence

🔍 Frameworks to Research During Learning
LangChain
Key Features
RAG Pipelines
Document Loaders
Vector Database Integration
Prompt Templates
Retrieval Chains
Best For
Enterprise RAG Systems
AI Assistants
Knowledge Retrieval Applications
LlamaIndex
Key Features
Data Connectors
Knowledge Indexing
Retrieval Optimization
RAG Workflows
Agent Integration
Best For
Enterprise Knowledge Bases
Document Search Systems
Agentic RAG Applications
ChromaDB
Key Features
Open Source Vector Database
Embedding Storage
Similarity Search
Lightweight Deployment
Best For
Learning RAG
Small-to-Medium Applications
AI Prototypes
🚀 Key Learning

Traditional AI answers from memory.

RAG answers from retrieved knowledge.

RAG is the bridge between Large Language Models and real-world enterprise data.

Part 2 – Agentic RAG & Intelligent Retrieval
🎯 Learning Objectives

By the end of Part 2, you will understand:

What is Agentic RAG
Traditional RAG vs Agentic RAG
Retrieval Planning
Multi-Step Retrieval
Query Rewriting
Reflection During Retrieval
Tool-Based Retrieval
Multi-Agent RAG
Enterprise Agentic RAG Architecture
Agentic RAG for MoM Insight 360
Agentic RAG for IntelliHire Resume Studio
Future of Agentic Knowledge Systems
🧠 1. What is Agentic RAG?

Traditional RAG retrieves information once and generates an answer.

Agentic RAG adds intelligence.

The agent can:

✅ Plan

✅ Search

✅ Evaluate

✅ Retrieve Again

✅ Reflect

✅ Improve Results

Traditional RAG
Question
    ↓
Retrieve
    ↓
Answer
Agentic RAG
Question
    ↓
Plan Search
    ↓
Retrieve
    ↓
Evaluate Results
    ↓
Retrieve Again
    ↓
Reason
    ↓
Answer

The agent actively participates in retrieval.

🧠 2. Why Traditional RAG Has Limitations

Traditional RAG assumes:

One Search
=
Enough Information

This is often false.

Example

User asks:

Why did revenue decrease in July?

A single search may retrieve:

Revenue Report

But not:

Doctor Performance
Appointment Conversion
Branch Trends
Budget Targets

Result:

Incomplete answer.

🧠 3. How Agentic RAG Solves This

Agentic RAG thinks before retrieving.

Example:

Question:

Why did July revenue decline?

Agent thinks:

Need Revenue Data
Need Doctor Performance
Need Branch Trends
Need Conversion Data
Need Budget Comparison

Multiple retrieval operations occur.

Result

More accurate reasoning.

🧠 4. Retrieval Planning

Before searching:

Agent creates a retrieval plan.

Example

User:

Compare July and August performance.

Agent Plan:

Step 1:
Retrieve July Revenue


Step 2:
Retrieve August Revenue


Step 3:
Retrieve KPI Metrics


Step 4:
Retrieve Forecast Data


Step 5:
Generate Insights

This is retrieval planning.

🧠 5. Query Rewriting

Users often ask vague questions.

Example:

How is business doing?

Agent rewrites:

Show:
Revenue Trend
Growth Rate
Branch Performance
Budget Achievement

Improved retrieval quality.

Benefits

✅ Better search results

✅ More context

✅ Better answers

🧠 6. Multi-Step Retrieval

Complex questions require multiple searches.

Example

User:

Which branch performed best this quarter and why?

Agent performs:

Search #1:
Quarter Revenue


Search #2:
Branch KPIs


Search #3:
Appointment Conversion


Search #4:
Doctor Contribution


Search #5:
Budget Achievement

Combines everything.

Result

Executive-level insight.

🧠 7. Reflection During Retrieval

Modern agents evaluate retrieved information.

Reflection Questions
Do I have enough data?


Is information complete?


Are results relevant?


Should I search again?

If not:

Retrieve Again

This is called Retrieval Reflection.

🧠 8. Tool-Based Retrieval

Agentic RAG can use tools.

Examples:

Tool 1

Database Query

SELECT Revenue
FROM Reports
Tool 2

API Call

Forecast API
Tool 3

Document Search

Policy Documents
Tool 4

Web Search

Market Trends
Agent Flow
Question
      ↓
Select Tool
      ↓
Retrieve Data
      ↓
Analyze
      ↓
Answer
🧠 9. Multi-Agent RAG

Large systems often use multiple agents.

Architecture
User Query
       │
       ▼
Supervisor Agent
       │
 ┌─────┼─────┐
 ▼     ▼     ▼


Research Analysis KPI
Agent   Agent  Agent


       ▼
Reporting Agent


       ▼
Final Response

Each agent retrieves different information.

Benefits

✅ Better scalability

✅ Specialized retrieval

✅ Higher accuracy

🧠 10. Agentic RAG Architecture
User Query
      │
      ▼
Planning Agent
      │
      ▼
Query Rewriter
      │
      ▼
Retriever
      │
      ▼
Vector Database
      │
      ▼
Reflection Agent
      │
      ▼
Reasoning Agent
      │
      ▼
Final Answer

This is becoming the standard enterprise architecture.

🏢 11. Enterprise Example – MoM Insight 360
User Question
Why did JP Nagar miss revenue target?
Revenue Agent

Retrieves:

Revenue Reports
KPI Agent

Retrieves:

ASK Rate
Conversion Rate
Forecast Agent

Retrieves:

Trend Analysis
Reporting Agent

Generates:

JP Nagar missed target due to:


- Lower ASK Rate
- Reduced Conversion
- Fewer Referrals
- Lower Doctor Utilization
Result

Actionable business insight.

🎯 12. Enterprise Example – IntelliHire Resume Studio
Recruiter Question
Find best candidate for Python Developer role.
Resume Agent

Retrieves:

Candidate Resumes
Skill Agent

Retrieves:

Skill Match Scores
Ranking Agent

Retrieves:

Ranking Data
Recommendation Agent

Retrieves:

Historical Hiring Data
Result
Top 5 Candidates
Ranked by:
- Skill Match
- Experience
- Interview History
- Success Probability
🧠 13. Agentic RAG vs Traditional RAG
Feature	Traditional RAG	Agentic RAG
Single Retrieval	✅	❌
Multi-Step Search	❌	✅
Planning	❌	✅
Reflection	❌	✅
Tool Usage	Limited	Extensive
Multi-Agent Support	❌	✅
Enterprise Readiness	Medium	High
Answer Quality	Good	Excellent
🧠 14. Future of Agentic RAG

Industry is moving toward:

Generation 1
LLM Only
Generation 2
RAG
Generation 3
Agentic RAG
Generation 4
Multi-Agent RAG
Generation 5
Autonomous Enterprise Agents

This is where enterprise AI is heading.

📚 Key Takeaways

✅ Traditional RAG retrieves once

✅ Agentic RAG plans retrieval

✅ Query rewriting improves search quality

✅ Multi-step retrieval improves accuracy

✅ Reflection validates retrieved information

✅ Tools expand knowledge sources

✅ Multi-Agent RAG enables specialized intelligence

✅ Enterprise AI is rapidly adopting Agentic RAG

✅ MoM Insight 360 can use Agentic RAG for executive analytics

✅ IntelliHire Resume Studio can use Agentic RAG for intelligent hiring recommendations

🔍 Frameworks to Research During Learning
LangGraph
Agentic RAG Features
Retrieval Planning
State Management
Reflection Loops
Multi-Step Workflows
Multi-Agent RAG
Best For
Enterprise Agentic RAG
Advanced AI Systems
CrewAI
Agentic RAG Features
Specialized Retrieval Agents
Shared Context
Collaborative Retrieval
Team-Based Reasoning
Best For
Multi-Agent Knowledge Systems
Business Automation
LlamaIndex
Agentic RAG Features
Advanced Retrieval
Knowledge Indexing
Agent Integration
Multi-Source Search
Best For
Enterprise Knowledge Platforms
Agentic Search Systems

🚀 Key Learning

Traditional RAG retrieves information.

Agentic RAG thinks about how to retrieve information.

This transforms AI from a passive knowledge retriever into an intelligent knowledge-seeking agent capable of planning, reasoning, reflecting, and delivering enterprise-grade answers.