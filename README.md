# Feliu Persistent Memory

Persistent operational memory for local AI agents built from an OpenAI export using RAG, FAISS, Ollama and Knowledge Graphs.

This repository documents a real local implementation: converting years of ChatGPT conversations into a reusable memory layer for local agents.

## Case Study

The original system was built from a full OpenAI export.

Validated project scope:

- Local conversation export processed offline
- Local RAG index
- Local Knowledge Graph
- Agent integration through Codebuff / Freebuff


## Goal

Build a persistent memory system that allows local AI agents to remember operational context across sessions while keeping the data local.

The system is designed to support:

- operational memory
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

- Local inventory and validation performed

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

- Retrieval validation performed with a local index

### Phase 7 - Knowledge Graph

Capabilities:

- entity discovery
- relationship mapping
- path finding
- network analysis

Validated graph scale:

- Local graph with entity and relationship queries

### Phase 8 - Agent Integration


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
- local indexes
- secrets
- environment files

Only architecture, methodology and reusable tooling should be shared.

## Lessons Learned

- The hard part is not creating a RAG index.
- The hard part is curating memory quality.
- Facts, assumptions, historical decisions and current rules must be separated.
- Persistent memory works better when it is structured, audited and regenerated under control.
- Local memory allows agents to preserve context while maintaining local control.

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

Future objective:

Persistent memory shared across multiple AI systems while keeping data local and under user control.

## Evidence levels and reproducibility

This repository is a **case study of a local implementation**. Its operational status describes the original local environment; it does not mean that a new clone can reproduce that environment without the private export, indexes, models and configuration.

| Claim | Evidence described here | Reproducible from this public repository? |
| --- | --- | --- |
| Historical export processing | Project phases and local artifacts | No: source export is private |
| Semantic retrieval | Local FAISS/Ollama validation described | Not independently established here |
| Knowledge-graph queries | Local graph validation described | Not independently established here |
| Recall after restart | Local restart validation described | Not independently established here |

### Suggested verification for a clean-room reproduction

1. Use synthetic documents, never personal ChatGPT exports.
2. Record source identifiers and hashes before ingestion.
3. Query known facts and deliberate negative controls; capture expected and observed results.
4. Restart the services and repeat the same queries.
5. Check duplicate ingestion, stale rules and missing provenance.
6. Publish only redacted commands, versions and aggregate outcomes.

**Security:** do not commit exports, embeddings, vector indexes, graph databases, tokens or machine-specific paths. This documentation is not a public benchmark or a turnkey installer.

## Current status versus roadmap

The phases above document historical work. Multi-agent sharing, additional model integrations and stronger provenance controls remain roadmap items until supported by published implementation evidence.
