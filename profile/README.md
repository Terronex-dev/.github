# Terronex

**Neural Memory for AI Systems**

## What We Build

**Engram** is a binary memory format for AI applications. Hierarchical storage, semantic search, multi-modal support, knowledge graphs. One file format that works across TypeScript, Python, Rust, and Go.

**Allo** is a neural memory assistant. Load any .engram file, search semantically, chat with your data. Works with local LLMs (Ollama) or cloud providers (Anthropic, OpenAI).

## Engram V2.1 — Spatial Intelligence

**From trees to graphs. From search to reasoning. Now with location.**

```typescript
// V2: Knowledge graphs
graph.addLink(createLink(studyId, claimId, 'supports'));
const evidence = graph.getLinkedNodes(claimId, 'supports');

// V2.1: Spatial queries
const nearby = spatialRecall(tree, {
  center: { x: 48.8566, y: 2.3522 },  // Paris
  radius: 500,                         // km
  metric: 'haversine'
});
```

| Feature | V1 | V2 | V2.1 |
|---------|----|----|------|
| Semantic search | ✓ | ✓ | ✓ |
| Typed links | ✗ | ✓ | ✓ |
| Graph traversal | ✗ | ✓ | ✓ |
| Spatial positions | ✗ | ✓ | ✓ |
| **Distance queries** | ✗ | ✗ | ✓ |
| **Geo (Haversine)** | ✗ | ✗ | ✓ |

Full specification: [SPEC_V2.md](https://github.com/Terronex-dev/engram/blob/main/SPEC_V2.md)

## Engram SDKs

| Language | Package | Version | Status |
|----------|---------|---------|--------|
| TypeScript | [@terronex/engram](https://www.npmjs.com/package/@terronex/engram) | **2.1.0** | V2.1 Spatial |
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
