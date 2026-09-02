Day 24 – CrewAI Fundamentals & Building Your First Multi-Agent Team
Part 1 – CrewAI Fundamentals
🎯 Learning Objective

By the end of this chapter, you should understand:

What CrewAI is
Why CrewAI was created
Core concepts of CrewAI
Agents, Tasks, Crews, and Processes
Sequential vs Hierarchical execution
CrewAI architecture
Agent, Task, and Crew attributes
How CrewAI can be applied in enterprise projects
How CrewAI fits into MoM Insight 360

CrewAI is one of the most popular frameworks for building Multi-Agent AI systems where multiple agents collaborate to achieve a common goal. It provides concepts such as Agents, Tasks, Crews, and Processes to organize AI teamwork.

1. Introduction to CrewAI

Before CrewAI, most AI applications looked like:

User
 ↓
LLM
 ↓
Answer

Example:

User:
What was our revenue last month?

LLM:
Provides answer.

This works for simple questions.

But enterprise systems require:

Data retrieval
Analysis
Validation
Reporting
Collaboration

A single AI agent becomes difficult to manage.

CrewAI solves this problem by organizing multiple AI agents into a team (Crew) that collaborates to complete tasks.

Traditional Software Team Analogy

Think about a software project.

You have:

Business Analyst
↓
Developer
↓
Tester
↓
Project Manager

Each person has a role.

CrewAI follows the same concept.

Research Agent
↓
Analysis Agent
↓
Validation Agent
↓
Reporting Agent

Together they solve a problem.

2. Why CrewAI?

As AI systems become more advanced, one agent may struggle with:

Too many responsibilities
Too many tools
Too much context
Too much reasoning

CrewAI addresses this by enabling specialized agents with defined roles and goals.

Problems With Single-Agent Systems
Problem 1

Context Overload

One agent
Must know everything
Problem 2

Tool Complexity

Database
API
Email
Excel
Dashboard

One agent handling everything can become inefficient.

Problem 3

Limited Scalability

As requirements grow:

One Agent
↓
Becomes Bottleneck
CrewAI Solution
Coordinator Agent
      ↓
 ┌─────────────┬─────────────┐
 │             │             │
Research    Analysis    Validation
 Agent       Agent        Agent
 │             │             │
 └─────────────┴─────────────┘
       ↓
Reporting Agent

Each agent becomes an expert.

3. Core Concepts

CrewAI is built around four main concepts:

Agent
Task
Crew
Process

Everything in CrewAI revolves around these four building blocks.

A. Agent

An Agent is an autonomous AI worker with:

Role
Goal
Responsibilities
Tools
Memory

CrewAI describes agents as autonomous units that can perform tasks, use tools, make decisions, collaborate, and maintain memory.

Example:

Revenue Analyst Agent

Role:

Revenue Analyst

Goal:

Analyze revenue performance.
Human Analogy
Employee
=
Agent

Examples:

Developer Agent
Tester Agent
Business Analyst Agent
Manager Agent
B. Task

A Task is a piece of work assigned to an agent.

CrewAI tasks define what should be done, who should do it, and the expected output.

Example:

Analyze August revenue.

Assigned To:

Revenue Agent

Expected Output:

Revenue summary report
Human Analogy
Task
=
Work Assignment

Example:

Prepare monthly sales report.
C. Crew

A Crew is a team of agents working together toward a common objective.

Example:

Revenue Agent
KPI Agent
Forecast Agent
Reporting Agent

Together:

Executive Intelligence Crew
Human Analogy
Department
=
Crew

Examples:

Finance Team
HR Team
Sales Team
D. Process

A Process defines how tasks are executed and coordinated across the crew. CrewAI supports sequential and hierarchical processes.

Human Analogy
Workflow
=
Process
4. Sequential Execution

This is the simplest process.

Tasks execute one after another.

Task 1
 ↓
Task 2
 ↓
Task 3
 ↓
Task 4

CrewAI executes tasks in the order they are defined when using a sequential process.

Example
Revenue Agent
 ↓
KPI Agent
 ↓
Forecast Agent
 ↓
Reporting Agent
Real Example
Collect Revenue
 ↓
Calculate KPIs
 ↓
Forecast Revenue
 ↓
Generate Report
Advantages

✅ Easy to understand

✅ Easy to debug

✅ Predictable

Disadvantages

❌ Slower

❌ No parallel processing

5. Hierarchical Execution

Manager-Worker model.

A manager agent coordinates work and delegates tasks based on expertise. CrewAI requires a manager model or manager agent for hierarchical execution.

Architecture
Manager Agent
      ↓
 ┌────┼────┐
 │    │    │
 A    B    C
Example
Executive Manager Agent
       ↓
Revenue Agent
KPI Agent
Forecast Agent

Manager decides:

Who should do what?
Advantages

✅ Scalable

✅ Flexible

✅ Enterprise-ready

Disadvantages

❌ More complex

❌ Requires coordination

6. CrewAI Architecture

High-level architecture:

User
 ↓
Crew
 ↓
Process
 ↓
Agents
 ↓
Tasks
 ↓
Tools
 ↓
Results
Detailed View
User Query
      ↓
Coordinator Agent
      ↓
Task Assignment
      ↓
Specialized Agents
      ↓
Tool Usage
      ↓
Results
      ↓
Final Report
7. Agent Attributes

CrewAI agents are typically defined using attributes such as Role, Goal, Backstory, Tools, and LLM configuration.

Role

Defines expertise.

Example:

Revenue Analyst
Goal

Defines objective.

Example:

Analyze revenue trends.
Backstory

Defines behavior and context.

Example:

20 years experience in healthcare finance.
Tools

Examples:

SQL Tool
Excel Tool
Search Tool
API Tool
Memory

Stores previous interactions.

8. Task Attributes

CrewAI tasks commonly contain description, expected output, assigned agent, tools, and context.

Description

What needs to be done?

Expected Output

Desired result.

Assigned Agent

Who performs the task?

Tools

Allowed tools.

Context

Input from previous tasks.

Example
Task:
Analyze August revenue.

Expected Output:
Branch-wise revenue report.

Assigned Agent:
Revenue Agent
9. Crew Attributes

Crews define the team structure and execution strategy. Typical attributes include agents, tasks, process, memory, and configuration.

Agents

Team members.

Tasks

Work assignments.

Process

Sequential or Hierarchical.

Memory

Shared knowledge.

Configuration

Runtime settings.

10. Enterprise Example
Sales Intelligence Crew
Sales Manager Agent
       ↓
Revenue Agent
Target Agent
Performance Agent
       ↓
Reporting Agent
Workflow
Sales Data
     ↓
Revenue Analysis
     ↓
Target Analysis
     ↓
Performance Analysis
     ↓
Executive Report
Output
Revenue exceeded target by 12%.

Top performing region:
South Zone.

Target achievement:
108%.
11. MoM Insight 360 Example

This is where CrewAI becomes relevant to your project.

Executive Intelligence Crew
Coordinator Agent
        ↓
Revenue Agent
        ↓
KPI Agent
        ↓
Forecast Agent
        ↓
Validation Agent
        ↓
Reporting Agent
Revenue Agent

Analyzes:

Revenue
Budget
Gap
DAR
FTW
KPI Agent

Calculates:

Branch Performance
Doctor Contribution
Department Contribution
PRO Contribution
Forecast Agent

Predicts:

Month End Revenue
Target Achievement
Growth Trend
Validation Agent

Checks:

Data Accuracy
Calculation Accuracy
Business Rules
Reporting Agent

Generates:

JP Nagar is behind budget by 5.4 Lakhs.

Current DAR required:
0.42 Lakhs/day.

Top Performing PRO:
Lohith.
12. Key Takeaways
CrewAI Formula
Agent
+
Task
+
Crew
+
Process
=
Multi-Agent System
Remember
Agent
=
Employee

Task
=
Assignment

Crew
=
Team

Process
=
Workflow
Enterprise Formula
Multiple Specialized Agents
+
Collaboration
+
Tools
+
Memory
=
Enterprise AI System
Day 24 Part 1 Summary

By completing this chapter, you now understand:

✅ What CrewAI is

✅ Why CrewAI exists

✅ Agent concept

✅ Task concept

✅ Crew concept

✅ Process concept

✅ Sequential execution

✅ Hierarchical execution

✅ CrewAI architecture

✅ Enterprise implementation approach

✅ MoM Insight 360 Crew design

Part 2 – Designing Our First Multi-Agent Project
🎯 Learning Objective

By the end of this chapter, you should understand:

How to design a Multi-Agent System
How to convert business requirements into agents
How agents collaborate
How CrewAI structures a project
How to define tasks
How to define workflows
How to create an enterprise-ready architecture
Why Are We Building This Project?

Before implementing AI in:

MoM Insight 360

or

IntelliHire Resume Studio

we need a small project that allows us to learn:

CrewAI
Agent Collaboration
Task Delegation
Workflow Design
Executive Reporting

without business complexity.

Project Name
AI Commerce Intelligence Crew

Dataset:

Kaggle

E-Commerce Sales Analytics Dataset
Business Problem

Assume you are the CEO of an e-commerce company.

Every morning you want answers such as:

Which category generated highest revenue?

Which products are performing well?

Which customers contribute most revenue?

What is the overall sales trend?

What actions should management take?

Instead of manually analyzing data,

we want AI agents to do the work.

Traditional Approach
CSV File
    ↓
Excel
    ↓
Pivot Tables
    ↓
Manual Analysis
    ↓
Management Report
Agentic Approach
CSV File
      ↓
Coordinator Agent
      ↓
 ┌────────────┬────────────┬────────────┐
 │            │            │
Sales      Customer    Product
Agent       Agent       Agent
 │            │            │
 └────────────┴────────────┘
       ↓
Reporting Agent
       ↓
Executive Summary
System Goal

Transform:

Raw Data

into

Insights

and

Recommendations
Step 1 – Understanding the Dataset

The dataset contains:

Orders
Customers
Products
Revenue
Payments
Categories
Locations
Business Dimensions

We can analyze:

Sales
Revenue
Orders
Growth
Customers
Repeat Customers
Top Customers
Customer Value
Products
Top Products
Top Categories
Product Trends
Payments
Payment Modes
Payment Preferences
Step 2 – Identifying Business Questions

Before creating agents:

Ask:

What questions must the system answer?
Sales Questions
What is total revenue?

Which month performed best?

Which category generated highest revenue?
Customer Questions
Who are top customers?

How many repeat customers exist?

Which customers contribute most revenue?
Product Questions
Which products are top sellers?

Which categories drive revenue?
Management Questions
What happened?

Why did it happen?

What should we do next?
Step 3 – Designing Agents

CrewAI starts with agents.

Agent 1
Coordinator Agent
Role

Project Manager

Goal

Coordinate all agents.

Responsibilities
Assign tasks

Collect outputs

Manage workflow

Create final response
Human Equivalent
Project Manager
Agent 2
Sales Intelligence Agent
Role

Sales Analyst

Goal

Analyze sales performance.

Responsibilities
Revenue Analysis

Sales Trends

Growth Analysis

Monthly Performance
Example Output
Electronics generated
38% of total revenue.
Agent 3
Customer Intelligence Agent
Role

Customer Analyst

Goal

Analyze customer behavior.

Responsibilities
Customer Segmentation

High Value Customers

Repeat Customers

Customer Revenue Contribution
Example Output
Top 10 customers
contributed 41%
of total revenue.
Agent 4
Product Intelligence Agent
Role

Product Analyst

Goal

Analyze product performance.

Responsibilities
Top Products

Top Categories

Product Revenue

Product Trends
Example Output
Electronics category
generated highest revenue.
Agent 5
Executive Reporting Agent
Role

Business Consultant

Goal

Generate executive insights.

Responsibilities
Summarize findings

Identify opportunities

Highlight risks

Recommend actions
Example Output
Revenue is growing steadily.

Electronics is the strongest category.

Focus marketing efforts
on repeat customers.
Step 4 – Designing Tasks

Agents need work.

Task 1

Assigned To:

Sales Intelligence Agent

Work:

Analyze Revenue

Analyze Monthly Trends

Identify Best Performing Period
Task 2

Assigned To:

Customer Intelligence Agent

Work:

Identify Top Customers

Analyze Customer Segments

Analyze Repeat Customers
Task 3

Assigned To:

Product Intelligence Agent

Work:

Analyze Product Performance

Analyze Category Performance
Task 4

Assigned To:

Executive Reporting Agent

Work:

Combine Findings

Generate Executive Summary

Generate Recommendations
Step 5 – Designing the Crew
Sequential Process

Simplest approach.

Sales Agent
      ↓
Customer Agent
      ↓
Product Agent
      ↓
Reporting Agent
Advantages
Easy

Predictable

Beginner Friendly
Recommended For
Version 1
Hierarchical Process

Manager model.

Coordinator Agent
      ↓
 ┌────┼────┐
 │    │    │
Sales Customer Product
Agent  Agent   Agent
Recommended For
Version 2
Step 6 – Project Folder Structure
AI-Commerce-Intelligence-Crew

│
├── data
│     └── ecommerce_sales.csv
│
├── agents
│     ├── coordinator_agent.py
│     ├── sales_agent.py
│     ├── customer_agent.py
│     ├── product_agent.py
│     └── reporting_agent.py
│
├── tasks
│     ├── sales_tasks.py
│     ├── customer_tasks.py
│     ├── product_tasks.py
│     └── reporting_tasks.py
│
├── crews
│     └── commerce_crew.py
│
├── outputs
│
├── notebooks
│
├── README.md
│
└── requirements.txt
Step 7 – Expected Workflow
Dataset
   ↓
Load Data
   ↓
Sales Agent
   ↓
Customer Agent
   ↓
Product Agent
   ↓
Reporting Agent
   ↓
Executive Summary
Example Executive Report
Total Revenue:
$2.8 Million

Top Category:
Electronics

Top Customer Segment:
Returning Customers

Revenue Growth:
12%

Recommendation:

Increase focus on
Electronics products.

Launch loyalty program
for repeat customers.
Step 8 – Mapping to MoM Insight 360

The same architecture can later become:

Coordinator Agent
        ↓
Revenue Agent
        ↓
KPI Agent
        ↓
Forecast Agent
        ↓
Validation Agent
        ↓
Reporting Agent
Learning Connection

This project combines everything learned so far:

Day 19
Agentic RAG

Day 20
Advanced RAG

Day 21
Agent Architectures

Day 22
MCP & Tool Calling

Day 23
Multi-Agent Systems

Day 24
CrewAI
💡 Key Takeaways
CrewAI Formula
Agent
+
Task
+
Crew
+
Process
=
Multi-Agent Application
Important Realization

A CrewAI project should not start with code.

It should start with:

Business Problem
↓
Questions
↓
Agents
↓
Tasks
↓
Workflow
↓
Implementation
Day 24 Completion Summary

After completing Part 1 and Part 2, you now understand:

✅ What CrewAI is

✅ Why CrewAI exists

✅ Agent, Task, Crew, Process

✅ Sequential Execution

✅ Hierarchical Execution

✅ CrewAI Architecture

✅ Multi-Agent Design

✅ AI Commerce Intelligence Crew Architecture

✅ How to apply CrewAI to MoM Insight 360