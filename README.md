JobFit – RAG-Based Resume & Interview Preparation System

JobFit is a GenAI-powered decision-support system that helps candidates tailor their resumes and interview preparation to specific job descriptions using semantic search and deterministic skill analysis.

Problem
Candidates often struggle to identify which projects to showcase and what skills to prepare for a job. Existing tools rely on keyword matching or generic advice, leading to poor guidance.

Solution
JobFit analyzes real job descriptions, matches them against a structured project portfolio using vector search, and generates direct, grounded instructions on resume selection and interview preparation.

How It Works
Scrapes and parses job descriptions using an LLM
Builds a semantic job-intent query
Retrieves relevant projects from a vector database (ChromaDB)
Computes covered and missing skills deterministically
Generates instruction-driven guidance using an LLM

Key Features
Semantic project matching (RAG-based)
Deterministic skill gap detection
Resume-ready project recommendations
Interview preparation guidance grounded in real projects

Tech Stack
Python, LangChain, Groq LLaMA, ChromaDB, Pandas

Why RAG
JobFit follows a task-oriented RAG approach where project data is retrieved first and all guidance is generated using retrieved evidence, preventing hallucination.

Disclaimer
This tool provides preparation guidance only and does not evaluate candidate eligibility or experience.
