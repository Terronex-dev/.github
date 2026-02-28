# Terronex

**Neural Memory for AI Systems**

Building the memory layer for intelligent applications. One format, multiple languages, production-ready.

## Engram

A binary memory format designed for AI systems. Hierarchical, searchable, multi-modal.

**Features:**
- Sub-millisecond semantic search (HNSW indexing)
- Hierarchical memory trees with parent/child relationships
- Multi-modal support (text, images, audio, code)
- Integrity verification (SHA-256)
- Streaming for large files
- Entity extraction and linking

**Performance:** 400x faster than brute-force search. 93.3% recall accuracy validated across 340+ real-world sessions.

## SDKs

| Language | Package | Repository |
|----------|---------|------------|
| TypeScript | [@terronex/engram](https://www.npmjs.com/package/@terronex/engram) | [engram](https://github.com/Terronex-dev/engram) |
| Python | engram-py | [engram-py](https://github.com/Terronex-dev/engram-py) |
| Rust | engram-rs | [engram-rs](https://github.com/Terronex-dev/engram-rs) |
| Go | engram-go | [engram-go](https://github.com/Terronex-dev/engram-go) |

All SDKs are cross-compatible. Files created in one language can be read by any other.

## Tools

| Repository | Description |
|------------|-------------|
| [engram-sdk](https://github.com/Terronex-dev/engram-sdk) | Converters and utilities (OpenStax textbook importer) |
| [engram-test-suite](https://github.com/Terronex-dev/engram-test-suite) | Cross-SDK validation fixtures |

## Applications

| Repository | Description |
|------------|-------------|
| [allo](https://github.com/Terronex-dev/allo) | Neural memory assistant with semantic search and LLM integration |

## Quick Start

**TypeScript:**
```bash
npm install @terronex/engram
```

**Python:**
```bash
git clone https://github.com/Terronex-dev/engram-py
```

**Rust:**
```toml
[dependencies]
engram = { git = "https://github.com/Terronex-dev/engram-rs" }
```

**Go:**
```bash
go get github.com/Terronex-dev/engram-go
```

## Links

- Website: [terronex.dev](https://terronex.dev)
- npm: [@terronex/engram](https://www.npmjs.com/package/@terronex/engram)

---

MIT licensed. Open source.
