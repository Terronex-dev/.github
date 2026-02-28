# Terronex

**Neural Memory for AI Systems**

## What We Build

**Engram** is a binary memory format for AI applications. Hierarchical storage, semantic search, multi-modal support, knowledge graphs. One file format that works across TypeScript, Python, Rust, and Go.

**Allo** is a neural memory assistant. Load any .engram file, search semantically, chat with your data. Works with local LLMs (Ollama) or cloud providers (Anthropic, OpenAI).

## Engram V2 — Now Available

**From trees to graphs. From search to reasoning.**

V2 adds typed relationships and knowledge graph traversal:

```typescript
// Create knowledge graphs
graph.addLink(createLink(studyId, claimId, 'supports'));
graph.addLink(createLink(finding1, finding2, 'contradicts'));

// Traverse relationships
const evidence = graph.getLinkedNodes(claimId, 'supports');
const path = graph.findPath(startId, endId);

// Auto-link similar content
graph.autoLinkSimilar(0.85);
```

| Feature | V1 | V2 |
|---------|----|----|
| Semantic search | ✓ | ✓ |
| Hierarchical tree | ✓ | ✓ |
| Typed links | ✗ | ✓ |
| Graph traversal | ✗ | ✓ |
| Spatial positions | ✗ | ✓ |
| Confidence scores | ✗ | ✓ |

Full specification: [SPEC_V2.md](https://github.com/Terronex-dev/engram/blob/main/SPEC_V2.md)

## Engram SDKs

| Language | Package | Version | Status |
|----------|---------|---------|--------|
| TypeScript | [@terronex/engram](https://www.npmjs.com/package/@terronex/engram) | **2.0.0** | V2 Complete |
| Python | [engram-py](https://github.com/Terronex-dev/engram-py) | 1.x | V1 (V2 compatible) |
| Rust | [engram-rs](https://github.com/Terronex-dev/engram-rs) | 1.x | V1 (V2 compatible) |
| Go | [engram-go](https://github.com/Terronex-dev/engram-go) | 1.x | V1 (V2 compatible) |

All SDKs pass the same test suite. V1 SDKs can read V2 files (V2 fields are ignored).

## Applications

| Project | Description |
|---------|-------------|
| [allo](https://github.com/Terronex-dev/allo) | Neural memory assistant with semantic search |

## Tools

| Project | Description |
|---------|-------------|
| [engram-sdk](https://github.com/Terronex-dev/engram-sdk) | Converters and utilities |
| [engram-test-suite](https://github.com/Terronex-dev/engram-test-suite) | Cross-SDK validation fixtures |

## Performance

- 400x faster than brute-force search
- Sub-millisecond retrieval (0.3ms average)
- HNSW indexing for O(log n) complexity

## Quick Start

```bash
# TypeScript (V2)
npm install @terronex/engram

# Python
pip install terronex-engram

# Rust
cargo add --git https://github.com/Terronex-dev/engram-rs

# Go
go get github.com/Terronex-dev/engram-go
```

## Links

- [terronex.dev](https://terronex.dev)
- [@terronex/engram on npm](https://www.npmjs.com/package/@terronex/engram)

---

MIT licensed. Open source. Patent pending.
