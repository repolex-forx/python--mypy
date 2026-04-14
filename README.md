# Repolex Knowledge Graph of python/mypy

RDF knowledge graph data for [python/mypy](https://github.com/python/mypy), parsed by [repolex](https://repolex.ai).

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
lexq download python/mypy
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 770d3ca4997032dc3a1c4f0b468e9f58e8f38505
│   │       ├── chunk-001.nq.gz
│   │       ├── chunk-002.nq.gz
│   │       └── chunk-003.nq.gz
│   ├── lsp
│   │   └── 770d3ca4997032dc3a1c4f0b468e9f58e8f38505.nq.gz
│   └── repolex
│       └── 770d3ca4997032dc3a1c4f0b468e9f58e8f38505
│           └── chunk-001.nq.gz
└── blob
    ├── 0020d9ceff468064122b223202b588f2133db7cf.nq.gz
    ├── 0031c72aea9f2ac5b811dc0605a828747559bb61.nq.gz
    ├── 0034d9e9bfff5e6d6c393b2d78a740670339bd71.nq.gz
    ├── 005020b8b6b30a5e195dfb2216699e7bd7d3e888.nq.gz
    ├── 009a4e68f67882d3adba47e0e5204cd062fb9335.nq.gz
    ├── 00a24b4eea07db49860884574712136b02f1cbb1.nq.gz
    ├── 00aae2ea814cb05059d459f74e4a989a3843282f.nq.gz
    ├── 00bcff68d4ff57209deab1a8569a1236de7294c1.nq.gz
    ├── 00cbe603a9b9176dc1125563a86f7ed52094f8b3.nq.gz
    ├── 00f234f9088eda25b9f2740b09aaa6e90d101e0a.nq.gz
    ├── 00fce56920b75430b11830df99d26d16a1eda068.nq.gz
    ├── 011a970d8bbcee7a0f3a647cba9dfe51659654d0.nq.gz
    ├── 014af8a0fd2ed53e80da576b32c1d7ea638a6318.nq.gz
    ├── 01bd734353a7b9977ab1d6f02f957dbb0bf5ecee.nq.gz
    ├── 0224035a7b61a5b0604f8c1a2b2d66d96c1d6c22.nq.gz
    ├── 02272d803c185211f008a8c027a96030df26dc42.nq.gz
    ├── 0234434b8c3de73cacb0f24e5c4fd1294bc3af0a.nq.gz
    ├── 02427ff4206203197cac7f88d1b12a49196b556d.nq.gz
    ├── 02caa44dce117296ee912ac3ca97221d4f3533c9.nq.gz
    ├── 034c795e712015bf2c4dc5cb40a2559f86b7c2d2.nq.gz
    ├── 036d858ddf69f0d9197b150ea4474134495d344f.nq.gz
    ├── 0383c3448d068dabe9ccff1e8f876f679d7613e3.nq.gz
    ├── 03b937261e22ad3978de15d3a4163f0f4bdb1b0c.nq.gz
    ├── 03c1eef3be3ffe287c1a2b2e1f98fd2212312730.nq.gz
    ├── 03d1d2e5c22038a4af9a9a3676b69ff65f2303bc.nq.gz
    ├── 047751fee1d2cde702c37f4d8f09067878ede8b3.nq.gz
    ├── 05426130d27263bd2c525696806eea15bd950d24.nq.gz
    ├── 054ad0ec0c4648b396bc1d6ca42945e40114f64c.nq.gz
    ├── 0559b33c33e2aceaea20692ff946e5c3d8ed3f51.nq.gz
    ├── 055f4def311cd88c7d076b40e83998b9dfd5f768.nq.gz
    ├── 058377accabcc2511b50d3e7f8d60023c832463e.nq.gz
    ├── 05844de8ecff70c6976efb7eaa6bebe689c78d5d.nq.gz
    ├── 05c3c8b3dd41ca29c58b98f1b81e56c9f62a3c70.nq.gz
    ├── 05daa64834f0f09abdc2a549762bdadb62324ed3.nq.gz
    ├── 06813c94308a08ee60ba258b7d7d5349a718cb22.nq.gz
    ├── 06dfcf5d0fbc15f4ef1f03405c59b0d203a55b78.nq.gz
    ├── 06e9f381a89ff8cd02d2b90844506c21209a1fbc.nq.gz
    ├── 06f8878a563e923184b71cfe05ab91a7f2194ce6.nq.gz
    ├── 070c59b1c166d2a3faf2f1c52414f7627fc5762c.nq.gz
    ├── 071b3aba5d330c6166170967ed69eaf9febdeb63.nq.gz
    ├── 072d1811c2a4cb1ae84a6ca24b5909afc5be562a.nq.gz
    ├── 07343414293c2c985692cd2f12fe2e9f7aef5a78.nq.gz
    ├── 074ab12792d99ae4b90b209c8e099efbdec8981a.nq.gz
    ├── 074df075b9727628f8edc86f5604598d9543d3a9.nq.gz
    ├── 0761baaa2830bdf8df98aa84225da983a56073e6.nq.gz
    ├── 077d4eebf7d398faf2c87b9574bc26047d1d8503.nq.gz
    ├── 079af85d51ee40e916875da0dd1ab0e3675048f3.nq.gz
    ├── 07e52d101206e57249df07de49bc54c854f0bae9.nq.gz
    ├── 07f9edf63cdd02fcd03ba6fe2d2b490cc39a627b.nq.gz
    ├── 080c5a402dbb0975ed1ebc56eecd3107ae5afd39.nq.gz
    ├── 083706507900b27adc3587d46a00eaff7e7c6ad8.nq.gz
    ├── 085cfc4f60a4b07a929d0871712511646530e1f9.nq.gz
    ├── 08619bf66351aebe0c7a6457fc076fbe59df9e19.nq.gz
    ├── 08c54c3bc376b056cd68e205198f65f9c6ea1b02.nq.gz
    ├── 08dc7b93692280173419ef0e01084846340004f6.nq.gz
    ├── 09062a635e63f24b23786f576f9c666f9a4e7d60.nq.gz
    ├── 090dfb960db6f5ad1f6a2e51fa0b276ec00f02ee.nq.gz
    ├── 0918d10ab1ef1953bdc634bbed6cf1e72ae3cd29.nq.gz
    ├── 093653553137fb315250b1450916b8413d305555.nq.gz
    ├── 09bf7fd980ec47f80290e891db7c4e2323d6ee38.nq.gz
    ├── 09e75e1ad4aa1494ee2c13d4814bc63ee31dec42.nq.gz
    ├── 0a0e180d635d7ecb1ccc55e15553046bb7dbaa38.nq.gz
    ├── 0a540610bc620a12038e6b8a5cf08ef3c280ee31.nq.gz
    ├── 0a7efcd45ff10fae9fe91783135a3fe477adda60.nq.gz
    ├── 0a99f0ae2e29b06dc89b85eabf8eec792d802dd3.nq.gz
    ├── 0a9ea32f5357dc43ad8bc1276ff9d2a825059887.nq.gz
    ├── 0aa699626525fcf7637284e080781725d707af9e.nq.gz
    ├── 0ab21fd29114fea768758af059b9f1c3ecba43af.nq.gz
    ├── 0adc7affb8cb416b6f35523907c36b6190f76c72.nq.gz
    ├── 0ae48b7c80d7ac278e10c20fa3c8acd7de3a55ac.nq.gz
    ├── 0af87658e59f2026d0e6a686283788dc87df9a6f.nq.gz
    ├── 0afb69bc0c99895ed139f3795d00561bf26a1f8d.nq.gz
    ├── 0aff1579b57f7513bc2bd8ff9a0874c2e31cd5fc.nq.gz
    ├── 0b13c8a5016d48082758581ef8e2bb8c250d4918.nq.gz
    ├── 0b20d5911151fb3a5d67ea456cdf6a8711c79721.nq.gz
    ├── 0b3fb9122c7b94ba01bb8c5047c8f83f0a005be7.nq.gz
    ├── 0b768908a4487c6c6a1c674ce899ae265eb9366e.nq.gz
    ├── 0bc5637b32708644fabb908a6ff17f255379e214.nq.gz
    ├── 0bced038664397d7734320ac47b5fa4510f6bf75.nq.gz
    ├── 0c4f1cb1fe599a5f09b0dfae9c307a32b1dd3063.nq.gz
    ├── 0c717b5d9a0e74efd0e96cc1b8094cc8c23fd2d6.nq.gz
    ├── 0c87444d18f441d4995ec43fd28f72b4ca162fc5.nq.gz
    ├── 0c93834fc23d48744070fb6a943ed4730a1c002d.nq.gz
    ├── 0caa6b8694b798f15a2a1825ac7b38d5c7eff031.nq.gz
    ├── 0cd37fe5f94532c363e31cf6215cc79210d1ac85.nq.gz
    ├── 0cdb340a63b7fcbc6ee4a7f1f3b9506c4bca042e.nq.gz
    ├── 0cf0edb32f86c66591b39f3cdbb22ee997ee6633.nq.gz
    ├── 0d3a0a7490a33b34df563477ada9f0bafb51592d.nq.gz
    ├── 0d8ac2d47491401637b0d29828c971fd791dd70d.nq.gz
    ├── 0ddeca7882cd109e8b398565b584f73dba1b1f9f.nq.gz
    ├── 0df2004186556593ebfb9093829226f3ef78c36d.nq.gz
    ├── 0df45ea22d336bdf0183e6a4559e85e9115fdb53.nq.gz
    ├── 0e02092a361c9d2aaed08cec17b8572af5ffd0ca.nq.gz
    ├── 0e1bb4165d99d87c8be185607928167604758e8c.nq.gz
    ├── 0e7f7ce165c3db031dba7c104d4dd159922cc611.nq.gz
    ├── 0e9a3a80ff0edf7675a436c5bfd034f28375a07f.nq.gz
    ├── 0ed729e24e439220d99063de7dcb25abc4b5d603.nq.gz
    ├── 0ef78d03e5f4a07e9e7f06f5a40eca9c55c4961b.nq.gz
    ├── 0f0d61a396d5f45cb89f378666c52fa59e858332.nq.gz
    ├── 0f13d0e810e91fe91999b790a48b3e23638b8d2a.nq.gz
    ├── 0f24d52e99912a6aad0c10def5131bfc543d6ab1.nq.gz
    ├── 0f2917764ba068934ed023d9f5a1936c882d7376.nq.gz
    ├── 0f3768d6dcf4d178586aae91131352dc3257eba2.nq.gz
    ├── 0f3cf05257408c60950fc462a2f2a3d5e6dcecde.nq.gz
    ├── 0f486b1d00464dddd2d759111dc59ed60e4cb81d.nq.gz
    ├── 0f62a4aa8b1a2ea8d71ef25988dc0c4d8b3d71df.nq.gz
    ├── 0f9d4343b63075e24171e066cc422ca025ad440a.nq.gz
    ├── 0fa1a4787087217e2ee1cd9b7b8ec35bffd20c19.nq.gz
    ├── 0fa81662dfbc1ab798d3c7188d20282a97c779f6.nq.gz
    ├── 0fb890d424b10fc289618e30fa6c8774182e68fe.nq.gz
    ├── 1003fda8d9ae86590dafd8120af0b6b342ee31d4.nq.gz
    ├── 10333d113a689e39934fe3f6e02bf8abca008ebd.nq.gz
    ├── 1060ee63c57df58574d01f4af0033bdc30efd5ef.nq.gz
    ├── 10784e7d402144a8b2de3cac07658632b9fae2d4.nq.gz
    ├── 10875a951fb422879e733a35a8c3799e5ad3b43d.nq.gz
    ├── 10991f26c408f89f1c78a2311d544408c2a965e3.nq.gz
    ├── 10eef2336a8343f9004f5a9212c197b1f4f26f6f.nq.gz
    ├── 10f475b352e662b7110340ad7738417120258687.nq.gz
    ├── 110b5bb85e43e34a7d017d206f8b1b467ab04ddd.nq.gz
    ├── 113145e395f62c8fe1a8ac23b75e8453530c782f.nq.gz
    ├── 11a93ca82d8df3fc10943cf75fa1b8ffc9f29043.nq.gz
    ├── 11c7286f5ed4283fb043288e98ffcc9c1a542150.nq.gz
    ├── 11e00213d05a74303939e30a1d670b9643f031dd.nq.gz
    ├── 11fa3635a2c7ab15aa7b0382922969122c5c59aa.nq.gz
    ├── 1227aa8978af232bb997b0b54ebf73768eb7131a.nq.gz
    ├── 122bf5df14e7c8af6ead435d776613d5d22733aa.nq.gz
    ├── 1260717489e41fb8ebc314c6ffce2b404d828ce0.nq.gz
    ├── 12aae33eaaf59550b2ba0ac1e62f51e18c868ed1.nq.gz
    ├── 12ed93f21223de2f53f5d64d1c001908930c82fd.nq.gz
    ├── 12fb191809e8630fbf48e7a26835b0554f9aaa63.nq.gz
    ├── 1323a55e9aad81b21a0b20a13229a1fa2a1d27d7.nq.gz
    ├── 13264487581f82433dadf18a99613a7d215fd448.nq.gz
    ├── 14148720269a4d93688450b8b0930346851fa883.nq.gz
    ├── 141f3ce143f690e09f4e9de72a79400f4c313c71.nq.gz
    ├── 146494df1bd6c3096e29056a9cc8f729364400e2.nq.gz
    ├── 1471267b24ee51a65def0e131c69cc3922630a35.nq.gz
    ├── 14721ca7a0cbae3ecf73ab5e64f9fa56ae9b8372.nq.gz
    ├── 14ceef550dab6dfb4d9e5c057ff5ccb1e8d27111.nq.gz
    ├── 14f691c9451f238540046c837896822893615c29.nq.gz
    ├── 153428148518e187c199d2b1b5da35136a6f7dd9.nq.gz
    ├── 153be5e2f6f996741b53558d8bc7825ec091699c.nq.gz
    ├── 15a82b1f719c654c38b89e31eb8ea55f6e94a0dd.nq.gz
    ├── 15b1065cb7a908b18aafd49f0f3439c5e47acf53.nq.gz
    ├── 15e717191ff058c01e426f174d88de31adc43080.nq.gz
    ├── 160f6c0365d63a3c6ab5005d1f4ddbe4d9b9c6a9.nq.gz
    ├── 161f14e8aea77adf08075ac3a67f128094a3124c.nq.gz
    ├── 1632256b747480cf124626ad70cb188e196824a0.nq.gz
    ├── 16684ff06956811b976f7d00c6c39946c9751e01.nq.gz
    ├── 16915423e47263f3e1ecf777c93f56668c82b7f0.nq.gz
    ├── 16cf0611a58ad36c3bfb051fcdf126ee3bc43e7c.nq.gz
    ├── 1714e01a2c284bb286774d5e5e94ae42329307c8.nq.gz
    ├── 172e57cf1a4b328e61cb169ebaa8aa6a0dcbc062.nq.gz
    ├── 17390b0c5a0ee9d0b84830a7e4e1b6d44715a390.nq.gz
    ├── 174f249913514ed6ba5edc421450a3ce2e7e7638.nq.gz
    ├── 1763c23182736ec16209666eb5b65e52ac0ba525.nq.gz
    ├── 1796a7e2160e43fad052a6395820f3c815025370.nq.gz
    ├── 179a31b63ff4ec257dcf9f817282bb914ab4c62c.nq.gz
    ├── 17c9e6597c9a55b383b483a24b4a9e10c8fd1153.nq.gz
    ├── 17ce4cd5965904ecf97461d86182086ff03de4ab.nq.gz
    ├── 17d4eef69af76219c1cee28609208ad728f2310b.nq.gz
    ├── 17d519cc8eeaeb4161f2d33b2d3cf6577280f0f2.nq.gz
    ├── 182e9cdf4a17dbfcb2f24d1261d8287c9d6b344b.nq.gz
    ├── 1838ec5d145b5372b6f02a19d1c73f939a09b4e6.nq.gz
    ├── 184015ffe7203d1ecd313586dccef953bb73621a.nq.gz
    ├── 1888a6595b61ba0536511ca925db976269b08307.nq.gz
    ├── 188bed3375bfd9e0861eb4e871902157f723a56e.nq.gz
    ├── 18a8a6457d757eed32b6f800ebc40189b3e48ea0.nq.gz
    ├── 18c5df033e2f671dc4406c44372b0f30246b7dba.nq.gz
    ├── 18d05a472688c226e44de0f863e80829f8341e5b.nq.gz
    ├── 1903d488f7bb38072dd8eab6d7d56689516645c3.nq.gz
    ├── 1909d80e3d18960961638fa5346af1ccf166f744.nq.gz
    ├── 1988edbef1f7bfaf7b700ac4312e82b35dda6dc7.nq.gz
    ├── 19a4a95eaeb0e4a19a19de7aa676313babdbbac9.nq.gz
    ├── 19d8117a621fcc4de8e2f1aa4f314005bdff017c.nq.gz
    ├── 1a29be7c836d1798d7c2f86909befe6d02ea0213.nq.gz
    ├── 1a61abac9732d1eab673061c10d8118c34281b28.nq.gz
    ├── 1a79fce59ab12219c706d38a74ef365713790e09.nq.gz
    ├── 1a7ed3348e126f8731c15daaa10ae409015d67df.nq.gz
    ├── 1a869438101fe19ba87876558f9a863547ed3004.nq.gz
    ├── 1ae551ecbf20d87023643445dbbf11e1be98a709.nq.gz
    ├── 1b180b9331971090e28f2003426b974dda6e3fa8.nq.gz
    ├── 1b1ec82032b4f7ef2461062ad84ef46538983e9f.nq.gz
    ├── 1b325b20d95bb3a2acc5e9c3b488a847d0e482c1.nq.gz
    ├── 1b38481ba000479a071973a8e56eeecffceb362c.nq.gz
    ├── 1b390e9c35043a8abfc31a8a06e9f7f0896f02d3.nq.gz
    ├── 1bb96e1a778688b1840fecee594e32b45d590010.nq.gz
    ├── 1bf1a59f7d3fb9ca32c7d075795da45b727a0cec.nq.gz
    ├── 1bf7db2f76e984bb65ee1c9ba9685a8e7f067dc5.nq.gz
    ├── 1c0b7756f29258eb7b67660ebe8b053c2992d3a8.nq.gz
    ├── 1c19bfb11e767306e223b877cd28244c71f6ece6.nq.gz
    ├── 1c27483782fb50e8b074547a6f614953409318e6.nq.gz
    ├── 1c27b55159593ae488b3a7e6ef3b1a8fc7bee185.nq.gz
    ├── 1c2d876486049b4cf5c058d2979115c5e470623c.nq.gz
    ├── 1c501e590f405dc13aaf50751bff78b92372b1e4.nq.gz
    └── 1c63bf6471dccc1c7aec2686bd90245412738560.nq.gz

8 directories, 200 files
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

[python/mypy](https://github.com/python/mypy)

---
*Parsed on 2026-04-14 by [repolex](https://repolex.ai)*
