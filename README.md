# Weekly Learning Progress

This repository documents my weekly learning progress for IST 343, with a focus on building practical technical capability for a GenAI-oriented project.

The learning direction is based on the Week 01 skill diagnostic and sprint planning documents. My current technical development track is **Modeling, Analytics or AI Development**, with emphasis on RAG, LangChain, LangGraph, evaluation, and responsible use of GenAI.

## Project Context

The project is expected to use retrieval-augmented generation and GenAI workflows to retrieve evidence from uploaded documents and support a maturity assessment process. The technical goal is not only to generate answers, but to build an evidence-grounded workflow where retrieval, validation, and human review can support reliable decision-making.

## Current Skill Baseline

From the Week 01 diagnostic:

- **Strong foundation:** programming and technical tools, including Java, Spring Boot, SQL, Git/GitHub, APIs, Redis, RabbitMQ, and full-stack development.
- **Working proficiency:** data understanding, data preparation, evaluation, and responsible use of GenAI.
- **Primary growth area:** hands-on AI application development, especially LangChain, LangGraph, RAG pipelines, agent workflows, and evaluation methods for LLM systems.

The highest-priority technical skill is **RAG and AI workflow development**, because the project needs to connect uploaded evidence with a structured GenAI assessment workflow.

## Repository Structure

```text
Weekly_Learning_Progress/
  Week01/
    M2 Project Skill Diagnostic_Wenxuan_Shen.docx
    M2 Skill Sprint Plant_Wenxuan_Shen.docx
  Week02/
    01_RAG_basic_demo/
      Document loading, text splitting, embeddings, Milvus, and a RAG knowledge-base case
    02_LangGraph/
      chapter01/
        LangGraph state, nodes, reducers, messages, and basic LLM workflow examples
      chapter02/
        Edges, routing, parallel execution, dynamic send, Command, fan-in, map-reduce, loops, retry, and cache
  Week03/
    00_Basic_RAG_Pipeline.ipynb
      A self-contained loading, splitting, chunking, TF-IDF vectorization, retrieval, and query demo
    01_LangGraph/
      chapter03/
        Persistence, checkpoints, state history, replay, forking, store, and context examples
      chapter04/
        Human-in-the-loop, interrupts, approvals, parallel execution, and tool-call examples
  Week04/
    LangGraph state, checkpoints, subgraphs, workflows, routing, and agent examples
  Week05/
  Week06/
  Week07/
  Week08/
```

## Learning Roadmap

| Sprint | Capability Focus | Project Need | Evidence to Produce |
| --- | --- | --- | --- |
| Sprint 1 | Build a basic end-to-end RAG pipeline | Retrieve relevant evidence from uploaded documents | Working demo, source code, retrieval examples, notes, and commits |
| Sprint 2 | Evaluate and improve retrieval quality | Improve the accuracy and reliability of evidence retrieval | Retrieval test cases, configuration comparisons, and error analysis |
| Sprint 3 | Integrate RAG into a controlled LangGraph workflow | Connect retrieval with assessment, validation, and human review | Workflow diagram, LangGraph code, test cases, and execution results |

## Current Focus

The basic local RAG pipeline in `Week03/00_Basic_RAG_Pipeline.ipynb` now demonstrates:

1. Creating and loading sample text documents.
2. Cleaning and splitting text into sentences.
3. Building overlapping word chunks.
4. Converting chunks and a query into TF-IDF vectors.
5. Ranking chunks with cosine similarity.
6. Building a grounded prompt and simple extractive answer with source attribution.

The notebook uses only the Python standard library, so it can be run from top to bottom without an API key or external vector database. The next step is to replace the local demo components with project documents, model-based embeddings, a persistent vector store, and an LLM generation call.

## Evidence Tracking

Each weekly folder should collect artifacts that show both learning and application. Useful evidence includes:

- Practice notebooks or scripts.
- Technical notes explaining concepts, decisions, and issues encountered.
- Retrieval examples and test questions.
- Configuration comparisons, such as chunk size, overlap, metadata use, retrieval strategy, or reranking.
- Error analysis and improvement notes.
- Project-facing prototypes or reusable components.

## Responsible GenAI Principles

This learning progress also tracks responsible and effective use of GenAI. Outputs from LLMs should be verified rather than automatically accepted. For this project, important quality concerns include hallucination, grounding, privacy, evaluation, and keeping human judgment in the decision-making loop.

## Intended Outcome

By the end of the sprint sequence, this repository should show a progression from basic RAG practice to a more reliable GenAI workflow that can process sample project documents, retrieve useful evidence, generate grounded responses, and support evaluation and human review.
