# Day 11 – Advanced RAG Patterns

## Learning Objective

Understand how modern enterprise RAG systems improve retrieval quality, reduce irrelevant context, increase answer accuracy, and scale effectively for production AI applications.

---

# 1. Why Basic RAG Is Not Enough

Naive RAG Workflow:

User Query
↓
Embedding
↓
Vector Search
↓
Retrieve Documents
↓
Context Injection
↓
LLM Response

Limitations:

- Irrelevant document retrieval
- Missing important documents
- Large context windows
- Duplicate information
- Poor ranking
- High token costs

---

# 2. Advanced RAG Architecture

User Query
↓
Query Enhancement
↓
Hybrid Search
↓
Reranking
↓
Metadata Filtering
↓
Context Compression
↓
LLM
↓
Final Response

---

# 3. Hybrid Search

Hybrid Search combines:

- Semantic Search
- Keyword Search

Formula:

Hybrid Search = Vector Search + Keyword Search

Benefits:

- Better recall
- Better precision
- Improved enterprise search

---

# 4. Reranking

Workflow:

Retrieve Top 20 Documents
↓
Reranker
↓
Select Top 5
↓
Send to LLM

Benefits:

- Improved relevance
- Lower token usage
- Better answer quality

---

# 5. Metadata Filtering

Example Metadata:

- Branch
- Department
- Doctor
- Year
- Month

Benefits:

- Faster retrieval
- Reduced search scope
- Improved accuracy

---

# 6. Query Transformation

User Query:

How is business doing?

Transformed Query:

Provide branch-wise revenue, appointment conversion and target achievement for the last 30 days.

Benefits:

- Better retrieval
- More accurate answers

---

# 7. Multi-Query Retrieval

Original Query:

How can I improve appointment conversion?

Generated Queries:

- Appointment conversion improvement
- Lead conversion strategies
- Patient conversion metrics
- Booking optimization

Benefits:

- Better coverage
- More comprehensive retrieval

---

# 8. Parent-Child Retrieval

Workflow:

Child Chunk Found
↓
Retrieve Parent Section
↓
Provide Full Context

Benefits:

- Better context
- Improved understanding
- Reduced ambiguity

---

# 9. Context Compression

Purpose:

- Remove duplicates
- Remove irrelevant information
- Reduce token consumption

Benefits:

- Faster responses
- Lower costs
- Better signal-to-noise ratio

---

# 10. RAG Evaluation Metrics

## Retrieval Precision

Relevant Retrieved
-------------------
Total Retrieved

## Retrieval Recall

Relevant Retrieved
-------------------
All Relevant Documents

## Other Metrics

- Answer Accuracy
- Groundedness
- Hallucination Rate

---

# 11. Advanced RAG in MoM Insight 360

Use Cases:

- KPI Definitions
- Revenue Reports
- Branch Reports
- ASK Rate Analysis
- Executive Summaries

Pipeline:

Query Enhancement
→ Metadata Filtering
→ Hybrid Search
→ Reranking
→ Context Compression
→ AI Response

---

# 12. Advanced RAG in IntelliHire

Sources:

- Resume
- Job Description
- Skill Matrix
- Hiring Guidelines
- Interview Feedback

Outputs:

- Match Score
- Strengths
- Skill Gaps
- Hiring Recommendation

---

# 13. Enterprise RAG Maturity Levels

Level 1 – Naive RAG

Level 2 – Hybrid Search

Level 3 – Hybrid Search + Reranking

Level 4 – Metadata Filtering + Query Rewriting

Level 5 – Agentic RAG

Agentic RAG enables AI systems to decide:

- What to search
- Where to search
- How much context to retrieve
- Which tools to use

---

# Key Takeaways

- Advanced RAG improves retrieval quality.
- Hybrid Search combines semantic and keyword search.
- Reranking improves relevance.
- Metadata Filtering improves precision.
- Query Transformation improves search quality.
- Multi-Query Retrieval improves coverage.
- Parent-Child Retrieval preserves context.
- Context Compression reduces costs.
- Evaluation metrics help measure effectiveness.
- Enterprise AI systems rely heavily on Advanced RAG.

---

# Day 11 Learning Outcome

A successful RAG system is not just about retrieval; it is about retrieving the right information, ranking it intelligently, and delivering only the most valuable context to the AI.