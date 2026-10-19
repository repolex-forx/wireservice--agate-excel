# Repolex Knowledge Graph of wireservice/agate-excel

RDF knowledge graph data for [wireservice/agate-excel](https://github.com/wireservice/agate-excel), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download wireservice/agate-excel
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 596ea9e9a757756c503a8de7203446ffd436ebc6
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 596ea9e9a757756c503a8de7203446ffd436ebc6
│           └── chunk-001.nq.gz
├── blob
│   ├── 0b62e04df3c1de2d60f86e90776b284901173196.nq.gz
│   ├── 123014908bebbfb7ecfa1d15daaceb272fabe05b.nq.gz
│   ├── 1368f2c65c2fa24dc6ef51bd40b2bf7b229144ae.nq.gz
│   ├── 20d07e467ab24b0c0ae9ece4604fd0f9006a914b.nq.gz
│   ├── 28c63eaa2d533f79c78104168e4251e924276716.nq.gz
│   ├── 2d280ce9d6526789a1b31410f3b80cc949753e81.nq.gz
│   ├── 426bb8a619dcb3ef0245df8f9cc2fc3f221cc149.nq.gz
│   ├── 43941de4376b013e022377a3160e0a494e9806e1.nq.gz
│   ├── 4c0acf64cf1c5487ef0661b833b9820a239929b4.nq.gz
│   ├── 52d5f6e1f9a309ed8f3f62da6e14a740acc9ee8f.nq.gz
│   ├── 56c50495c63461b5ff2f473a8e92ef5a93011c65.nq.gz
│   ├── 595d201bbf692a1a132a213e2acc280c934ac231.nq.gz
│   ├── 59a8941e6bf9d1cb2ead62a5d3f5feb37c6e5ad5.nq.gz
│   ├── 5fe87e5451301fbd1273793bfea44d9f7b42eca6.nq.gz
│   ├── 6d13fb5faaa10d3c6eaaa10e67a44be792fb2912.nq.gz
│   ├── 79ea49ca02dc2fa0c59e887a3db3b1c8b433cdac.nq.gz
│   ├── 839e32696e0c4a043b83180c0bfb144f17896587.nq.gz
│   ├── 85a5c7e65e6d172e305f0d4b37ccff891c82c2ca.nq.gz
│   ├── 86d492877a2313b2a2650a9eb61c9aad87a409f1.nq.gz
│   ├── 8f557394919bbef5583a720b199d0fbd329a9efb.nq.gz
│   ├── 9deaf2be429b10232ec5fec4d83e1e7f29fca292.nq.gz
│   ├── 9f36d0d70fce754046f85e789b6a66d52a1788f8.nq.gz
│   ├── a522d950751f20be4baf6f6f76cfe730038e0bd8.nq.gz
│   ├── a669e4fa308643e106c6b3df7d0387783eeaa4f2.nq.gz
│   ├── a78e982f7e738c8f219f2833f2ef99862c2ea9d3.nq.gz
│   ├── b3ecd330d692b4e79f0b325419caa926027b618c.nq.gz
│   ├── bda5336c4a1d23a530bbb71d9a373dd3f36c6906.nq.gz
│   ├── c375686c857b409c44990eaf3e288871143bdb46.nq.gz
│   ├── c687a552540267cadb79ace95c25dc5603cb7899.nq.gz
│   ├── ceeccfbf7315d6af9a645497b8fd40a2854f90f6.nq.gz
│   ├── d28ed2483899b1b3d87f4d977d2b0267e8d8c2a7.nq.gz
│   ├── d7c082b7ecc2af320afa1a8c50e175f6248d83a3.nq.gz
│   ├── d7fb9478b0febcdacfbc77d37aa1ca076c8483e7.nq.gz
│   ├── d8b41db63b6c3e407806b0a7e0d1db9e6e1fcb3d.nq.gz
│   ├── d8ff73c4c603a5b785393838c7da5e1d6c4ee1e1.nq.gz
│   ├── e0feb12d716793ed286277ca753d631b59b9e41a.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e910dd47a103bc01d78677748bb50d868b12db82.nq.gz
│   ├── ea8753a6a34dc1322a15ba5b5dd3102eb64b0119.nq.gz
│   └── ffd1183afae022b3ebe09f47af3ba2c5c6925974.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 596ea9e9a757756c503a8de7203446ffd436ebc6.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 48 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[wireservice/agate-excel](https://github.com/wireservice/agate-excel)

---
*Parsed on 2026-10-19 by [repolex](https://repolex.ai)*
