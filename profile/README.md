# Terronex

**Neural Memory for AI Systems**

## What We Build

**Engram** is a binary memory format for AI applications. Hierarchical storage, semantic search, multi-modal content, integrity verification. One file format that works across TypeScript, Python, Rust, and Go.

**Allo** is a neural memory assistant. Load any .engram file, search semantically, chat with your data. Works with local LLMs (Ollama) or cloud providers (Anthropic, OpenAI).

## Engram SDKs

| Language | Package | Status |
|----------|---------|--------|
| TypeScript | [@terronex/engram](https://www.npmjs.com/package/@terronex/engram) | Published |
| Python | [engram-py](https://github.com/Terronex-dev/engram-py) | Ready |
| Rust | [engram-rs](https://github.com/Terronex-dev/engram-rs) | Ready |
| Go | [engram-go](https://github.com/Terronex-dev/engram-go) | Ready |

All SDKs pass the same test suite. Files are fully cross-compatible.

## Applications

| Project | Description |
|---------|-------------|
| [allo](https://github.com/Terronex-dev/allo) | Neural memory assistant with semantic search |

## Tools

| Project | Description |
|---------|-------------|
| [engram-sdk](https://github.com/Terronex-dev/engram-sdk) | OpenStax textbook converter (10+ books supported) |
| [engram-test-suite](https://github.com/Terronex-dev/engram-test-suite) | Cross-SDK validation fixtures |

## Content

The OpenStax converter transforms CC BY 4.0 college textbooks into .engram files:

- U.S. History (32 chapters, 2,971 nodes)
- Biology
- Chemistry  
- Anatomy and Physiology
- Astronomy
- Economics
- Calculus
- Algebra and Trigonometry

## Performance

- 400x faster than brute-force search
- Sub-millisecond retrieval (0.3ms average)
- 93.3% recall accuracy across 340+ sessions
- HNSW indexing for O(log n) complexity

## Quick Start

```bash
# TypeScript
npm install @terronex/engram

# Python
git clone https://github.com/Terronex-dev/engram-py

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
