# Repolex Knowledge Graph of UKPLab/emnlp2025-aspects-in-reviews

RDF knowledge graph data for [UKPLab/emnlp2025-aspects-in-reviews](https://github.com/UKPLab/emnlp2025-aspects-in-reviews), parsed by [repolex](https://repolex.ai).

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
rlex download UKPLab/emnlp2025-aspects-in-reviews
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 39076968c4630fd20cbe318a533ce90e981dd762
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 39076968c4630fd20cbe318a533ce90e981dd762
│           └── chunk-001.nq.gz
├── blob
│   ├── 064d9bc0092a1b828ea8a673d78d1ae935072fbf.nq.gz
│   ├── 083ba08a28b752f3e9a0b8eb0dfdde7d4e132e3a.nq.gz
│   ├── 099b2835bfbdbabd4765b952463ac7f499e4f2f1.nq.gz
│   ├── 0c7261116c1ef8f95717ed8b5496bb5eb86bc872.nq.gz
│   ├── 109d27f06f5456fc093f28f5f4ea848c8d1b670e.nq.gz
│   ├── 1f2916db875cdb4db98d1fba75244fb309ea1f4e.nq.gz
│   ├── 261eeb9e9f8b2b4b0d119366dda99c6fd7d35c64.nq.gz
│   ├── 2c0c6b0ed4b1f8d154dffb067f4ae0ddd68554ea.nq.gz
│   ├── 2e014ae45debf941d13b59e57a18164d3a705f78.nq.gz
│   ├── 48ee8f09f029231642516c7655e9d3d13f47151d.nq.gz
│   ├── 4c87cfef6715cfb9cc23fcc7e1d79c0a5a058102.nq.gz
│   ├── 63b52e9a63cbe1e088dc7aea69fa1c750a4bd608.nq.gz
│   ├── 6ed474a40c424fb4482c18f177a2658373fb9526.nq.gz
│   ├── 712961a6ad27c6f86db03617652c7a68ffab49f2.nq.gz
│   ├── 7d3d68c6ad0c30c94e802984365e58cda35a3c00.nq.gz
│   ├── 80f6d4c3ab6dc25be8ba6a638386ce59884fc8d3.nq.gz
│   ├── 933dd8a4dde1e1a04ee192100a57a2b48adbd069.nq.gz
│   ├── a484d5784ab5787226e4818fc3d259cb09be86e9.nq.gz
│   ├── ad970ac32ed7c373798b1b69c3e17d781963119d.nq.gz
│   ├── b07c5e294015c70ad881f52a30c8998e4875a9c1.nq.gz
│   ├── b609d6e39aa89e52132a6185b0f5fbe568b1df83.nq.gz
│   ├── c255a5de84e8e23765045b32f3021f96aa3629fd.nq.gz
│   ├── cd276f35ecaea96913d0fa9c68e8e61c872a0f45.nq.gz
│   ├── ce75872921e514af5bdb6a8cf7e63b78c7f5d141.nq.gz
│   ├── ce7a3be2fa6878f679ee4742cab3cb6ec529109d.nq.gz
│   ├── cf956f0547e0e135dee989e3f5dc30c052dd6840.nq.gz
│   ├── cfa62682d75e34b0586e2a09abd578ee75042820.nq.gz
│   ├── d327559693fe615443eaadf5aaf33aa150c80997.nq.gz
│   ├── d62f84cbc7e482a3878e791ea56525ea8e54c02a.nq.gz
│   ├── d88b93162b7d218ca366ef965f1002721226b0a0.nq.gz
│   ├── dbb08956a2116f6588f98085ba20cb04dd97982f.nq.gz
│   ├── ddafa12d14f816be7a8ba4a68f46383d36d8b2c0.nq.gz
│   ├── e14b012126a9a5d4e8572c34f2be681f4a194e32.nq.gz
│   ├── e1c9acc27b5ca2f93d40ca066f1941fb6dac94e4.nq.gz
│   ├── e231f1e789bd168761e4352d8d22dc6fdb9e04f1.nq.gz
│   ├── e4f62bfbe06135503f03b109b3e67ffcc9a59906.nq.gz
│   ├── e865f12dde28ac05eaabffbf70b6c25a26665a81.nq.gz
│   ├── ebf57b418bbd3a51c50992557d8405b80e0eb0f1.nq.gz
│   ├── f080a586ba30795abf47ef0c2794ba9f709c4ba9.nq.gz
│   ├── fe4e7bf204ca25f474efb5930b371f751f1346ed.nq.gz
│   └── ff1476a74ec96627849ca235554f7ee6931dcc5f.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 39076968c4630fd20cbe318a533ce90e981dd762.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 47 files
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

[UKPLab/emnlp2025-aspects-in-reviews](https://github.com/UKPLab/emnlp2025-aspects-in-reviews)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
