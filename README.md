# Feliu Persistent Memory

Persistent operational memory for local AI agents built from an OpenAI export using RAG, FAISS, Ollama and Knowledge Graphs.

This repository documents a real local implementation: converting years of ChatGPT conversations into a reusable memory layer for local agents.

## Case Study

The original system was built from a full OpenAI export.

Validated project scale:

- 3,163 conversations
- 156,135 messages
- 6.4 GB export
- 89.7 MB extracted text
- Around 24,000 referenced attachments
- Local RAG index
- Local Knowledge Graph
- Agent integration through Codebuff / Freebuff
- First deployment target: R2, my local operational agent

Private data is not included in this repository.

## Goal

Build a persistent memory system that allows local AI agents to remember operational context across sessions while keeping the data local.

The system is designed to support:

- personal operational memory
- project memory
- decision history
- editorial rules
- entity and relationship discovery
- semantic search
- graph-based queries
- future integration with multiple daily-use AI tools

## Architecture

OpenAI Export
↓
Safe local copy
↓
Inventory and statistics
↓
Knowledge extraction
↓
Unified memory document
↓
RAG index
↓
Knowledge Graph
↓
Unified query wrapper
↓
Agent context loader
↓
Persistent operational memory

## Local Stack

- Linux
- Python
- Ollama
- nomic-embed-text
- FAISS
- Knowledge Graph
- Codebuff / Freebuff

## Project Phases

### Phase 1 - Export Preparation

- Preserve original OpenAI export
- Work only on copies
- Create isolated workspace
- Maintain traceability
- Keep full backups

### Phase 2 - Inventory and Statistics

Results:

- 3,163 conversations
- 156,135 messages
- 89.7 MB extracted text
- Around 24,000 referenced attachments

Generated artifacts:

- INVENTARIO.md
- ESTADISTICAS_CONVERSACIONES.md
- ESTRUCTURA_EXPORT.md

### Phase 3 - Knowledge Extraction

Extracted:

- rules
- decisions
- projects
- entities
- relationships

### Phase 4 - Unified Memory

Generated:

- unified memory document
- timeline
- expanded knowledge graph
- operational rules
- historical decisions
- historical projects

### Phase 5 - Coverage and Audit

Validated:

- coverage
- contradictions
- missing topics
- false positives
- knowledge gaps

The audit showed that memory quality is more important than memory volume.

### Phase 6 - Local RAG

Components:

- Ollama
- nomic-embed-text
- FAISS

Validated results:

- 144 chunks
- 768 embedding dimensions
- sub-second retrieval

### Phase 7 - Knowledge Graph

Capabilities:

- entity discovery
- relationship mapping
- path finding
- network analysis

Validated graph scale:

- 124 entities
- 78 relationships

### Phase 8 - Agent Integration

Integrated into R2 using:

- CLAUDE.md as context loader
- query.py for semantic retrieval
- graph_query.py for relationship queries
- consultar.py as unified wrapper
- regenerar.py for controlled regeneration and reindexing

### Phase 9 - Persistent Memory Validation

Validated after system restart.

Capabilities confirmed:

- automatic context loading
- semantic retrieval
- graph queries
- historical project recall
- relationship discovery
- local operation

## Security Model

This repository does not include:

- OpenAI exports
- personal conversations
- private memory files
- personal identifiers
- private knowledge graphs
- local indexes
- secrets
- environment files

Only architecture, methodology and reusable tooling should be shared.

## Lessons Learned

- The hard part is not creating a RAG index.
- The hard part is curating memory quality.
- Facts, assumptions, historical decisions and current rules must be separated.
- Persistent memory works better when it is structured, audited and regenerated under control.
- Local memory allows agents to preserve context without uploading private data.

## Roadmap

- Multi-agent memory sharing
- n8n integration
- cross-model memory layer
- Gemini integration
- Claude integration
- additional local agents
- stronger distinction between verified facts, outdated rules and inferred knowledge

## Status

Current status: operational.

First production deployment:

R2 - Local Operational Agent

Future objective:

Persistent memory shared across multiple AI systems while keeping data local and under user control.

