# Repolex Knowledge Graph of block/drift

RDF knowledge graph data for [block/drift](https://github.com/block/drift), parsed by [repolex](https://repolex.ai).

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
rlex download block/drift
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── ca4a55360da354801162b56f407638b55d4ca008
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── ca4a55360da354801162b56f407638b55d4ca008.nq.gz
│   └── repolex
│       └── ca4a55360da354801162b56f407638b55d4ca008
│           └── chunk-001.nq.gz
├── blob
│   ├── 034174592cbd9153eb5006436b8395902a5ff67d.nq.gz
│   ├── 03f305e2563b28605613da1672ce807b622c0984.nq.gz
│   ├── 080447d3f2be4c4a86dc053688f61754ef3e1b5d.nq.gz
│   ├── 16ab6deb524489b055c6bcedf07292b92142699f.nq.gz
│   ├── 1824bb11a32c9143e2a5d4826c5097dca5ffcaa4.nq.gz
│   ├── 18858dfdd1f1da50b284ee20334a5a1a8043c135.nq.gz
│   ├── 1dfd4cd6f9bb515346c83fc6a93890bfa566a16c.nq.gz
│   ├── 1e8794608a77c43457f8f26088d9b1adaf91e8bd.nq.gz
│   ├── 1f2ffac583beafcfd05bf0e3e853ba3c235e4db9.nq.gz
│   ├── 2995b7d83245a1d93ab1d478099d1be66321f14f.nq.gz
│   ├── 31a8fb873a2e45914013d000c6d32fcca8dcc254.nq.gz
│   ├── 327a276a5e276d5e849e7a194028710e549dcf27.nq.gz
│   ├── 3a0ae95feebacc4e3a188dd0445685a5723dcbda.nq.gz
│   ├── 3ba13e0cec6cbbfd462e9ebf529dd2093148cd69.nq.gz
│   ├── 3e04de731f2044203b6f43f651f01a2953a6d3fb.nq.gz
│   ├── 3fd37b2c71427808117fc21c1835ef23817d254b.nq.gz
│   ├── 410cd72f6fb4a2c5d7cc2a6fa28cb973a5279371.nq.gz
│   ├── 47b40de721b97dafdaa9df33b3b551e826d9d230.nq.gz
│   ├── 4ba064d8dd25c561d66809c9f9a34367cf0bd29c.nq.gz
│   ├── 509b211767e4895c8b15e1ebada5ffc3be38ddb6.nq.gz
│   ├── 5581c8f32077983023a8814506ccd9aaf310b495.nq.gz
│   ├── 578b446a1456d40da8bd24c30013fa0de2370b1d.nq.gz
│   ├── 628cc9f0765abe25fa1a59892ed9ec0efcf583fc.nq.gz
│   ├── 629d70a9d855a74f325234a9883c07f912d8d35f.nq.gz
│   ├── 6779023a8589fba050b5aab024e4ce588adad26b.nq.gz
│   ├── 6bccf43368fd7c96d9c659562a5142b8b8cb98a1.nq.gz
│   ├── 6f412e2e790f21c066abdff7fe003ee23f3aaf2c.nq.gz
│   ├── 75d5fe0b26c69019f0a53fd95e54edacfae096e7.nq.gz
│   ├── 7e420fb6a8d4b84fed12c0f38803aaae434de4c5.nq.gz
│   ├── 8369a59719c9917afb5915876dad27a5e561060b.nq.gz
│   ├── 862ee3c28647e7a58801a75236855c269c1448ae.nq.gz
│   ├── 889e00b122d56e5f0d5ca442996c03742c345377.nq.gz
│   ├── 89fb992705a28d8d9edbb7d20b8c3d20a7030c09.nq.gz
│   ├── 8a29790731f42ac6a9b455b1b7a5cb64dc8a1d7c.nq.gz
│   ├── 8e6893658131f531e0b94e0c343d65e90447c451.nq.gz
│   ├── 8eb7787a2e52069f31f38881c2121de0fa20da23.nq.gz
│   ├── 9183dc75e49169f82e2049c07189e38cc3251b2f.nq.gz
│   ├── 9557c06724a079e58b40244de9cb918622ce7871.nq.gz
│   ├── 9582fc588754f78d9875691a3bd5e674295436b3.nq.gz
│   ├── 9b664dfaffaa3b7508195d1d35050667daf0939b.nq.gz
│   ├── a0cd57fd3ad1fbfb6a9132eac23e161752968f28.nq.gz
│   ├── a0fa2d2bf71db2b05a8b39b1385f89dda1c48eb7.nq.gz
│   ├── a2265f246b2681875f81042671998678c21f8e6d.nq.gz
│   ├── a2f32604b80bc86ec0c362dd201103b085cd4c47.nq.gz
│   ├── a5c958c7a3178a89156d8738661b5797af9c8d39.nq.gz
│   ├── a9fbd8002b05d42994b699512105da04b1e249e5.nq.gz
│   ├── aaea77afd6b1eeb2525dae1f90ea7c9d21aa123e.nq.gz
│   ├── b185e74284cb9f71fcf0a8b62414e1384d9407a6.nq.gz
│   ├── b51e591c782e4909bf5495ea0e895fe2a0c64bde.nq.gz
│   ├── b90359e47b1b47fba055a77364cc2aff46f1e746.nq.gz
│   ├── bae33c80e1f1c54c790f08827bf399e7f266a7bf.nq.gz
│   ├── be6e297dc321be3ad8fc83e2e9f8aa21b56f1384.nq.gz
│   ├── be8a67f18fc886076a23567477ef596a72d991a5.nq.gz
│   ├── bf7398433d85dbc28bffd0cd890d54ae911e7891.nq.gz
│   ├── c50914037a55e215b899820e00d99f8d25086814.nq.gz
│   ├── c7c5bd665c06a038b41ce0b46fca972b3d35a87b.nq.gz
│   ├── ce38719a50f4838211dbede6b814ffc349825d82.nq.gz
│   ├── cf5f53880aca9e2f75e87a4fd072547af9e45dba.nq.gz
│   ├── d0583495ccab24c94b3a89389812bd1177c25816.nq.gz
│   ├── d8921e513009bba84f75909c1e9d2502e1fb0078.nq.gz
│   ├── d8a3abee7ec07cafe41ab6729e59b5adc142791f.nq.gz
│   ├── e26aa035c84785c40e24a8e7adc0a29974075d3e.nq.gz
│   ├── e3439b4d89e16379454e8293b98cc6ac849489c8.nq.gz
│   ├── ea68d4a242e9a2980b6f71f745b9be77f2e524c5.nq.gz
│   ├── ea758221c909b5335a4d2f673012e988fa1417cb.nq.gz
│   ├── eb7e3c656caf9f20d08c43b98138bfff27dd13bb.nq.gz
│   ├── ec01bd616cd1a2077970a36e44ddbc0e3da0387f.nq.gz
│   ├── f20bc68dddd03e0db8ccffef6497c3d69e94a73f.nq.gz
│   ├── f25e8be0847f9a4c6fb7a20a25a6c11863d8acd6.nq.gz
│   ├── f2859656bd9df21890ba5e9ec19df73613d03e07.nq.gz
│   ├── f2aa0734a8718122f32be59da5e1b83f738bb3ec.nq.gz
│   └── fb1a8438723750dae15adafb95680badca693e37.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── ca4a55360da354801162b56f407638b55d4ca008.nq.gz
├── filetree
│   └── ca4a55360da354801162b56f407638b55d4ca008.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 82 files
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

[block/drift](https://github.com/block/drift)

---
*Parsed on 2026-10-01 by [repolex](https://repolex.ai)*
