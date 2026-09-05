# Repolex Knowledge Graph of repolex-ai/pan

RDF knowledge graph data for [repolex-ai/pan](https://github.com/repolex-ai/pan), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download repolex-ai/pan
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── d92f3db1f1b1a997d6290d1208e231d9e455c9d8
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── d92f3db1f1b1a997d6290d1208e231d9e455c9d8.nq.gz
│   └── repolex
│       └── d92f3db1f1b1a997d6290d1208e231d9e455c9d8
│           └── chunk-001.nq.gz
├── blob
│   ├── 00b77d37c3fcba1e67f35ce736b766ec2e514ec1.nq.gz
│   ├── 2907fdb947c8eafc44907d2c3de85df8b0ffaa33.nq.gz
│   ├── 2be44260c7f596f819fff6ea078fb8efd4502704.nq.gz
│   ├── 35b22ffd92d47b7cedf61cf467a91d83f71924b8.nq.gz
│   ├── 43103733cd184e449d39d71a1ec54caa34997106.nq.gz
│   ├── 474803eadab89b7a5ac01df674edbf1d04f43937.nq.gz
│   ├── 47879f451cc5f7a5af0467c67ec6c209dfd5eb19.nq.gz
│   ├── 4c3f14b624b168eafc8cd72beed7f2342cfbf027.nq.gz
│   ├── 56d7029f77c5d721bb61f422f30a689da44a8d40.nq.gz
│   ├── 5998fe7ad44cc0a340db66bdf326190007546419.nq.gz
│   ├── 5b637777e7c89fcb2d6af6ab11d344505cfd99a3.nq.gz
│   ├── 5f1a59bc79bfb8268731f4e74527be926bf60017.nq.gz
│   ├── 699a03d0e1cf0807e40854c54dcd6d809084e2da.nq.gz
│   ├── 71f669853a7fcb2518ef80ab55b12a3559191523.nq.gz
│   ├── 80a7e11050324f14acc0488ea90f5d76360d4bd8.nq.gz
│   ├── 80da415287440ffd12c274c741102e15f79ca02c.nq.gz
│   ├── 811043bfbba311cb97473468bec424fe3c341320.nq.gz
│   ├── 964c711d30f5386a98bcccc2e47dbac969860d30.nq.gz
│   ├── 9c13794df6523f190c0c1e1d01a9c437353da521.nq.gz
│   ├── a0cc2e51ab600723cbb4f2b0013278135d983d32.nq.gz
│   ├── a64e84fb5b52d8cbb179ca1270be848cf4bce557.nq.gz
│   ├── ae5e3e19c55ce599c7de51dece39da559ca504e6.nq.gz
│   ├── af0e8920b3adee483fbccbb87519fa5b88f3fd20.nq.gz
│   ├── af503962641c3b210a96a34aac72b9d0a805df28.nq.gz
│   ├── b63c2803a6bfc8b10d7c85a4ad09cdef5d7ef70e.nq.gz
│   ├── bc573929ebf390822f897603c8fe188c3ee1870e.nq.gz
│   ├── ca0fcbe68a4bc6cf233723effd1b1ab5eebdff0e.nq.gz
│   ├── e0037b4547c23bd35c60f167e3e3b92a12ee1839.nq.gz
│   ├── ecb5c7307c69d3dbfc2f96312336932b6e452d40.nq.gz
│   ├── efc85af98340a2a05ce502f27b3e3ca2b2118dc1.nq.gz
│   └── f230f93f00b6acb813ff85e0d2a6b92ee630a7fc.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── d92f3db1f1b1a997d6290d1208e231d9e455c9d8.nq.gz
├── filetree
│   └── d92f3db1f1b1a997d6290d1208e231d9e455c9d8.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 39 files
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

## Source repository

[repolex-ai/pan](https://github.com/repolex-ai/pan)

---
*Parsed on 2026-09-05 by [repolex](https://repolex.ai)*
