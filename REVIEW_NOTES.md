# WebPilot AI — Technical Review Notes

## Project Overview

WebPilot AI is a website-aware chatbot prototype that allows website owners to provide a URL, index website content, and embed a chat widget on their site. Visitors can ask questions about the indexed content and receive answers with source links.

## Implemented Capabilities

- Website URL onboarding.
- Website crawling and content indexing.
- JavaScript embed snippet generation.
- Website-specific chat widget with source links.
- Optional pasted-content onboarding.
- Sample Acme Store website for demonstration.
- Local SQLite-based storage and search.
- Offline demonstration mode using a mock LLM and local hashing embeddings.

## Demo Configuration

The project is configured for local demonstration without requiring an external model API key. The mock LLM and local hashing embeddings are intended to demonstrate the workflow, not to represent production-grade language generation or semantic retrieval quality.

## Production Readiness Considerations

Before deploying to production, consider implementing:

- Stronger authentication and authorization for website owners.
- Tenant isolation, usage quotas, and rate limiting.
- A durable background job queue for crawling and indexing.
- Monitoring, logging, and error tracking.
- Production-grade URL validation and SSRF/DNS-rebinding protections.
- Evaluation of answer quality, retrieval relevance, latency, and source attribution.
- Appropriate data retention and security controls.

## Scope

This repository demonstrates the core website-chatbot workflow. Production deployment, operational safeguards, and answer-quality validation require additional implementation and testing.
