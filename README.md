# Repolex Knowledge Graph of jazzband/django-superform

RDF knowledge graph data for [jazzband/django-superform](https://github.com/jazzband/django-superform), parsed by [repolex](https://repolex.ai).

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
rlex download jazzband/django-superform
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 92b4d9ea2c891d422abe97600cd281c2bf0d1d3c
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 92b4d9ea2c891d422abe97600cd281c2bf0d1d3c
│           └── chunk-001.nq.gz
├── blob
│   ├── 00f7a5809457f74a49c7dccf6c6d3c67c0127e5d.nq.gz
│   ├── 039259c5e76dd96470f60d451f3c92b08c08965d.nq.gz
│   ├── 0713beb4bdd49b3c71edd942679b2e7ecf461f49.nq.gz
│   ├── 0dbaa50262e79d81822b592611e777eb07207d99.nq.gz
│   ├── 1641ec95a071386e83288d3cce09375a27353405.nq.gz
│   ├── 1f7d0a52685065432f9a230f81d004e0b1b35cb6.nq.gz
│   ├── 24da9f16a14007fe1868011b333f3c79b51ecae7.nq.gz
│   ├── 327f0025403c453bd73b623c4748f844451f2b98.nq.gz
│   ├── 3398441feafa339a213b0806622da56775b4d4ce.nq.gz
│   ├── 35916ac9d17c196cdc3e12f406af672f7f6d9285.nq.gz
│   ├── 3b05cf41cea684cf7f93ed7b366c03281b7ec69d.nq.gz
│   ├── 45b87d33ddedc31a6f5919d49f3b909d253cceee.nq.gz
│   ├── 498da523be2dce892e046c6610f7a943302c66ea.nq.gz
│   ├── 49c7e42758fc58b3faf6fea4ba69bf4abf1ace38.nq.gz
│   ├── 4a00b475012718bfe9e6f8e0fd21d29bbb048948.nq.gz
│   ├── 4cf1c859630043a8b4552584579c8b61f4556609.nq.gz
│   ├── 50269fcd3196032bbb0290bc60797a80b789b880.nq.gz
│   ├── 692fb578e20be7a2f3c3fb083a6826eeef264a4c.nq.gz
│   ├── 6eebf7895f0070cf9dcdb3b8aa6e2bf018e5df65.nq.gz
│   ├── 710b3c9897de48a141d00f8dcc6455d3274c8186.nq.gz
│   ├── 85843e8144ac58569eca4821fe755c4b74376368.nq.gz
│   ├── 9273bb9c7f3e0bf98f0617498d529b49479d7a57.nq.gz
│   ├── 947ed45e93d5910305a0580cf21602edf26f28b9.nq.gz
│   ├── a48278a70f4a090a3a255f965f651939a457d76f.nq.gz
│   ├── a9774b62ff0ca1c3ba3c87a7cd93bfa246537d37.nq.gz
│   ├── ab55a88f84c476e470d51b34460c07ac5b21483b.nq.gz
│   ├── ac2d0229f632858cf356c29eb0cb8c6c577bf30a.nq.gz
│   ├── b213c956622f432f3674f161b44d7255eafab6ea.nq.gz
│   ├── b91a52bca31e084bf8a2012042d15a2ad98de84c.nq.gz
│   ├── c57306200c3018225567247f4b853ee3101e45d6.nq.gz
│   ├── c9e63e70aabf5964705c8f24fe9602b78ba5eb9a.nq.gz
│   ├── cb64aef44bdd9997fa29e8e2392155a31bda7fde.nq.gz
│   ├── d854431b14439d9a199a47751f15c68ac5ccf5b8.nq.gz
│   ├── d9e113ec685b92b018297dd2f200341d1fba01f9.nq.gz
│   ├── e12276223cd6746db3bd70691df23f786a16c6b5.nq.gz
│   ├── e53560bd8c307434a467bfd4fb7479b12f654ddd.nq.gz
│   ├── e58a932b469407967da49925c571a8ac6a081d53.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── f2c251ebcc9e28156b59acd89ef9615530221eba.nq.gz
│   ├── f9f0965b9e95b7664bd42dc7a5f0c17e7a20a8b4.nq.gz
│   └── fa4a29127f2c109000d5b064a1b3884fbef31f1b.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 92b4d9ea2c891d422abe97600cd281c2bf0d1d3c.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 49 files
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

[jazzband/django-superform](https://github.com/jazzband/django-superform)

---
*Parsed on 2026-10-10 by [repolex](https://repolex.ai)*
