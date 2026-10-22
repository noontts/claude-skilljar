# Claude API Learning Notes

Notes and notebooks from following the
[Building with the Claude API](https://anthropic.skilljar.com/claude-with-the-anthropic-api)
course on Anthropic Skilljar.

## Course outline

1. Introduction
2. Accessing Claude with the API: API keys, requests, multi-turn chat, system prompts, temperature, streaming, structured data
3. Prompt evaluation: eval workflow, generating test datasets, running evals, model-based and code-based grading
4. Prompt engineering techniques: being clear and direct, being specific, XML tags, providing examples
5. Tool use with Claude: tool functions and schemas, message blocks, multi-turn tool use, text edit and web search tools
6. RAG and agentic search: chunking, embeddings, BM25, multi-index pipelines
7. Features of Claude: extended thinking, images, PDFs, citations, prompt caching, code execution and the Files API
8. Model Context Protocol: servers, clients, tools, resources, prompts
9. Anthropic apps: Claude Code and computer use
10. Agents and workflows: parallelization, chaining, routing, agents vs workflows
11. Final assessment
12. Wrapping up

## Progress

| Section | Status | Notes |
| --- | --- | --- |
| 3. Prompt evaluation | In progress | [prompt_evals/](prompt_evals/) |

## Repository layout

```
.
├── deepseek_chat.ipynb          # Chat experiment using the DeepSeek API
├── prompt_evals/
│   ├── dataset.json                     # Generated eval dataset
│   ├── 001_prompt_evals.ipynb           # Eval workflow, starting point
│   ├── 001_prompt_evals_fns.ipynb       # Helper functions for the eval
│   ├── 001_prompt_evals_grader.ipynb    # Model-based / code-based graders
│   └── 001_prompt_evals_complete.ipynb  # Complete eval walkthrough
├── .env.example                 # Template for required environment variables
└── .gitignore
```

## Setup

1. Create and activate a virtual environment:

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

2. Install dependencies for the notebooks you want to run (for example `jupyter`, `anthropic`, `python-dotenv`).

3. Copy the env template and add your API key:

   ```bash
   cp .env.example .env
   ```

   `.env` is git-ignored, so keys are never committed.

4. Open a notebook in VS Code or Jupyter and run the cells.
