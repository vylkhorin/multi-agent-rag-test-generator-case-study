# multi-agent-rag-test-generator-case-study
Case study of an AI-powered Test Plan Generator using Multi-Agent Systems, RAG, AWS Bedrock LLMs, and Vector Search for automated software testing workflows.




# AI Test Plan Generator - Multi-Agent RAG System (Case Study)

## 📌 Overview

AI Test Plan Generator is an AI-powered application designed to automate software test plan creation using **Large Language Models (LLMs)**, **Multi-Agent AI Orchestration**, and **Retrieval-Augmented Generation (RAG)**.

The system analyzes requirements, documentation, and knowledge sources to automatically generate comprehensive and structured test plans with requirement traceability and quality metrics.

This project demonstrates how Generative AI can be applied in Quality Engineering workflows to improve productivity, reduce manual effort, and enhance testing consistency.

---

## 🔒 Confidentiality Notice

The original project was developed during my **Software Engineering Internship in the API Security Quality Engineering (QE) team at Thales (Imperva)**.

Due to company confidentiality policies and intellectual property restrictions:

- ❌ Production source code cannot be shared
- ❌ Internal repository access cannot be provided
- ❌ Live deployment/demo URL cannot be made public
- ❌ Internal prompts, configurations, credentials, and business logic cannot be disclosed

This repository is a **public technical case study** created to demonstrate the engineering concepts, architecture, AI workflows, and technical learnings behind the project.

This repository does NOT contain:
- Company-owned code
- Internal APIs
- Proprietary data
- Customer information
- Production configurations

---

# 🎯 Problem Statement

Enterprise Quality Engineering teams spend significant time manually creating test plans by analyzing:

- Product requirements
- Jira epics and stories
- Technical documentation
- Existing knowledge bases
- Security guidelines

Manual test plan creation can be:

- Time-consuming
- Repetitive
- Difficult to scale
- Dependent on domain expertise

The goal of this project was to explore how **Generative AI** can assist QE teams by automatically creating structured, requirement-aware test plans.

---

# 🚀 Solution

The AI Test Plan Generator uses a multi-agent AI workflow where specialized agents collaborate to:

1. Gather relevant context
2. Understand requirements
3. Retrieve supporting knowledge
4. Generate test scenarios
5. Validate coverage
6. Produce structured outputs

---

# ✨ Key Features

- 🤖 Multi-agent AI orchestration
- 🧠 Retrieval-Augmented Generation (RAG)
- 📚 Document-based knowledge retrieval
- 🔍 Semantic vector search
- 📝 AI-powered test case generation
- 📊 Requirement coverage analysis
- 📈 Quality metrics generation
- ⚡ Real-time progress tracking
- 📄 Structured Excel test plan output

---

# 🏗️ High-Level Architecture


```text
                    User Input
                        |
                        |
                        v
              Frontend Application
                 (React.js)
                        |
             REST API + WebSocket
                        |
                        v
              Backend Application
              (Python + FastAPI)

                        |
        +---------------+---------------+
        |                               |
        v                               v

 Multi-Agent System              RAG Pipeline

        |                               |

        |                       Document Processing
        |                               |
        |                       Vector Embeddings
        |                               |
        |                       Semantic Search
        |                               |
        +---------------+---------------+

                        |
                        v

                    LLM Engine

                        |
                        v

              Generated Test Plan

        +---------------+---------------+
        |               |               |
        v               v               v

 Test Plan Sheet   Requirements    Metrics Sheet
```


---

# 🤖 Multi-Agent Architecture

The system follows an agent-based design where each AI agent performs a specialized responsibility.

---

## 1. Orchestrator Agent

Responsible for managing the complete AI workflow.

### Responsibilities

- Coordinates all agents
- Processes gathered context
- Generates final test scenarios
- Controls test plan creation pipeline

---

## 2. Requirements Agent

Responsible for requirement understanding.

### Responsibilities

- Analyze feature requirements
- Extract acceptance criteria
- Identify functional scenarios
- Prepare structured requirement context

---

## 3. Knowledge Retrieval Agent

Responsible for retrieving relevant information.

### Responsibilities

- Search knowledge sources
- Retrieve relevant document chunks
- Provide additional context to LLM

---

## 4. Review Agent

Responsible for quality validation.

### Responsibilities

- Analyze generated test cases
- Validate requirement coverage
- Identify missing scenarios
- Generate quality metrics

---

# 📚 Retrieval-Augmented Generation (RAG)

The RAG pipeline improves AI generation quality by providing relevant external knowledge.

## Workflow

```text

Documents

    |
    v

Document Processing

    |
    v

Text Chunking

    |
    v

Embedding Generation

    |
    v

Vector Database

    |
    v

Semantic Retrieval

    |
    v

LLM Context

    |
    v

AI Generated Test Plan

```

---

# 📊 Generated Output

The final output is generated in structured Excel format.

---

## Test Plan Sheet

Contains:

- Test Case ID
- Test Scenario
- Preconditions
- Test Steps
- Test Data
- Expected Result
- Priority
- Test Category

---

## Requirements Sheet

Contains:

- Requirement ID
- Requirement Description
- Requirement Mapping
- Coverage Status
- Traceability Details

---

## Metrics Sheet

Contains:

- Total Test Cases
- Requirement Coverage
- Test Quality Metrics
- Gap Analysis Summary

---

# 🛠️ Technology Stack

## Backend

- Python
- FastAPI
- REST APIs
- WebSocket
- SQLAlchemy


---

## Frontend

- React.js
- Vite
- Axios
- CSS3


---

## AI / LLM

- AWS Bedrock
- Claude Models
- Multi-Agent AI
- Prompt Engineering


---

## RAG & Vector Search

- LangChain
- Vector Embeddings
- PostgreSQL
- pgvector
- Semantic Search


---

## DevOps

- Docker
- Kubernetes
- CI/CD Concepts


---

# 📈 Key Engineering Concepts

Implemented concepts include:

- Agentic AI system design
- Context-aware generation
- Vector similarity search
- LLM orchestration
- Async processing
- Real-time communication
- Cloud-native architecture
- Scalable backend design

---

# 🎓 Learning Outcomes

Through this project, I gained practical experience in:

- Building enterprise-style Generative AI applications
- Designing AI agent workflows
- Developing RAG-based systems
- Working with LLM integrations
- Building scalable APIs
- Applying AI in software testing
- Understanding API Security QE workflows

---

# ⚠️ Disclaimer

This repository is intended only as a **technical case study and learning showcase**.

The actual implementation was developed as an internal enterprise project.

All proprietary implementation details, internal resources, and confidential information have been removed.
