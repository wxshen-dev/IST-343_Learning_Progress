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
  Week04/
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

The immediate learning goal is to build a basic RAG pipeline that can:

1. Load sample documents.
2. Split text into chunks.
3. Generate embeddings.
4. Store vectors in a vector database.
5. Retrieve relevant chunks for a user question.
6. Pass retrieved context to an LLM for grounded answer generation.
7. Inspect retrieved chunks and identify common retrieval errors.

Week 02 materials currently support this goal through RAG practice notebooks and LangGraph workflow examples.

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
