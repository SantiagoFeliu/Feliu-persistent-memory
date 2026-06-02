# Architecture

## Overview

The objective of the architecture is to transform historical AI conversations into reusable operational memory for local agents.

## High Level Flow

AI Export
↓
Inventory
↓
Knowledge Extraction
↓
Unified Memory
↓
Embeddings
↓
RAG Index
↓
Knowledge Graph
↓
Query Layer
↓
Agent Integration
↓
Persistent Memory

## Components

### Inventory Layer

Responsibilities:

- conversation discovery
- message counting
- attachment analysis
- metadata extraction

### Knowledge Layer

Responsibilities:

- rule extraction
- decision extraction
- project extraction
- entity extraction
- relationship extraction

### Memory Layer

Responsibilities:

- memory consolidation
- traceability
- source preservation

### Semantic Layer

Responsibilities:

- embeddings
- semantic retrieval
- context expansion

### Graph Layer

Responsibilities:

- entity relationships
- path discovery
- network analysis

### Agent Layer

Responsibilities:

- context loading
- memory retrieval
- memory-assisted responses

## Design Principles

- Local first
- Source preservation
- Traceability
- Regeneration over manual editing
- Security by default
