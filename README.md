# LLM Engineering and Mastery

A practical, project-based roadmap for building reliable applications with
large language models (LLMs).

## What this repository covers

- **Foundations:** tokens, embeddings, transformers, context windows, and
  sampling
- **Application patterns:** prompting, structured output, tool calling, agents,
  and retrieval-augmented generation (RAG)
- **Production engineering:** evaluation, observability, latency, cost,
  security, and responsible deployment
- **Mastery projects:** progressively larger systems that turn each concept
  into a measurable capability

## Learning path

1. **Understand the model** — learn how tokenization, attention, embeddings,
   and decoding affect application behavior.
2. **Build a baseline** — create a small chat application with explicit
   prompts, configuration, error handling, and response logging.
3. **Add reliable interfaces** — use schemas, validation, retries, and
   deterministic tests for structured responses and tool calls.
4. **Ground responses in data** — implement document ingestion, chunking,
   retrieval, citations, and an evaluation set for a RAG application.
5. **Measure quality** — define task-specific metrics, regression tests, and
   human-review workflows before optimizing the system.
6. **Operate safely** — address prompt injection, data exposure, access
   control, rate limits, cost, and model/version changes.

## Engineering principles

- Start with a simple baseline and measure before adding agents or complex
  orchestration.
- Keep prompts, model settings, retrieved context, tool inputs, and outputs
  observable and versioned.
- Treat model output as untrusted input: validate it at every application
  boundary.
- Prefer small, composable components over a single opaque “agent.”
- Build evaluation into the development loop, not after deployment.

## Suggested capstone

Build a source-grounded assistant for a bounded document collection. It should
return structured answers with citations, refuse unsupported claims, expose
latency and token-cost metrics, and pass a versioned evaluation set in CI.

## Status

This repository is currently a learning roadmap and project starting point.
Future implementations should add one focused example at a time, together
with its evaluation and operational documentation.
