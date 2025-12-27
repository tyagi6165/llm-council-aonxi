# LLM Council – Aonxi Interview Challenge (n8n)

This repository contains an n8n-based implementation of a minimal LLM Council.

## What this does
- 3 LLM agents generate independent answers
- 2 judges evaluate answers using a rubric (non-generative)
- Safety gating before final output
- Structured Decision Object with confidence, risks, and citations
- Persistent audit log via Google Sheets

## Implementation
- Platform: n8n
- Core logic: n8n workflow JSON
- No model training required

## Non-Automated Design Decision
Final decision approval is intentionally not automated to allow human oversight in high-stakes decisions.

## How to use
1. Import the JSON workflow into n8n
2. Configure OpenAI credentials
3. Run the workflow with a test question
