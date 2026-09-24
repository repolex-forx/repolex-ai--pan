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
│   │   ├── 5fe090ca163977a45ec62a29e3905538ec899232
│   │   │   └── chunk-001.nq.gz
│   │   ├── c8b37eb2eb25bb2e783da4dd10f2347c0635727c
│   │   │   └── chunk-001.nq.gz
│   │   └── d92f3db1f1b1a997d6290d1208e231d9e455c9d8
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   ├── c8b37eb2eb25bb2e783da4dd10f2347c0635727c.nq.gz
│   │   └── d92f3db1f1b1a997d6290d1208e231d9e455c9d8.nq.gz
│   └── repolex
│       ├── c8b37eb2eb25bb2e783da4dd10f2347c0635727c
│       │   └── chunk-001.nq.gz
│       └── d92f3db1f1b1a997d6290d1208e231d9e455c9d8
│           └── chunk-001.nq.gz
└── blob
    ├── 003d663f6feda7bb8609960b075d55d3d97b0ca3.nq.gz
    ├── 00b77d37c3fcba1e67f35ce736b766ec2e514ec1.nq.gz
    ├── 00e28fe43f58548f20a82517de8f5b8b6f69bfd4.nq.gz
    ├── 020fa0c6a5c9206f4039ab0caac0ee45d2a2b9a3.nq.gz
    ├── 027c0c72bc3b85eec82af5a962ada85d081ce97c.nq.gz
    ├── 037aae32a1b46feabbd3cbcb69e22ff9e296a4f7.nq.gz
    ├── 058d5fad0b82614d299263853a94f70943b38e0b.nq.gz
    ├── 06821fbd82254ce7131c434ac39cbfdb22a15a3e.nq.gz
    ├── 06ce656ed10a0af21f1ae339b00ff2030dedeb58.nq.gz
    ├── 06d0736550a64240a5fbeb2b813b2d1ba12b0e44.nq.gz
    ├── 0723486e243362ded5994a2979c0b50d4458e43b.nq.gz
    ├── 08db51fb37b0526d73c2279f35a28282d7008e32.nq.gz
    ├── 0d12a1d070776d915aa66efc929171472657bc4b.nq.gz
    ├── 0d9d59251ee30a1e33a2c70b87e16d010d7f5fef.nq.gz
    ├── 0e5e0190b4c202327ce744ff42f363465e971ccc.nq.gz
    ├── 0f176d21bc64b31a8ff3eb6e0e3e176e70713fcc.nq.gz
    ├── 101d1b3240960623faa96b129e81a100d95e1a29.nq.gz
    ├── 1086943653307f9b7cace59710cfa5b1d6d902f7.nq.gz
    ├── 10bde3e55d6ec8c56a1085054ddcef2baa1d794d.nq.gz
    ├── 12c230ac813caa3f631a3034286cbd2d6a322409.nq.gz
    ├── 16cd681236b52688eb51b5d094d12b708abf9331.nq.gz
    ├── 19925e6feb6236bcf78107800d16d1fcbeb3d76d.nq.gz
    ├── 1c0e928f15eadbd5d3c1ac3e51d16eb5889ba9ad.nq.gz
    ├── 1c156adea92411a8a1ff79c5fe99c3bffaf778ac.nq.gz
    ├── 1e1bcef6c0bf7794cd568e036dafcdac37b8b608.nq.gz
    ├── 1f0647c9dcb2c98f550d888034748427990d15ec.nq.gz
    ├── 1f5c27a989efa62be38b5c7e192d9ade4f0d5858.nq.gz
    ├── 2055c547b8abfedc7739a9a35db8ccd2d4a43d22.nq.gz
    ├── 24f736a12499a3eaf6a520bd2eeff02bb84e58e0.nq.gz
    ├── 26a71fe76147a267907679f98947e7a78ab33f06.nq.gz
    ├── 2907fdb947c8eafc44907d2c3de85df8b0ffaa33.nq.gz
    ├── 2be44260c7f596f819fff6ea078fb8efd4502704.nq.gz
    ├── 2cfab15730eb97970e90530634a66f213740fdff.nq.gz
    ├── 2e7dc53350103dbd0705fc43d8e3a619b7676ac9.nq.gz
    ├── 2ed89b8a6e4bcbab8b077a9e751fc6e9415b51a1.nq.gz
    ├── 302262bc5bc6db9e5fcb722f478b1b89c1eaefd3.nq.gz
    ├── 33fb4cc9a1a71ed6f81fdcc48cb66b35b8d36e9a.nq.gz
    ├── 34607da8da46efd46ab2561d9c7f297a6ed76980.nq.gz
    ├── 348cf6d17f47461e31f5374bcdc0b3be5b24d234.nq.gz
    ├── 35b22ffd92d47b7cedf61cf467a91d83f71924b8.nq.gz
    ├── 3af94eb00154369b1294a74f09854b0eacfb7226.nq.gz
    ├── 3b7e4a71a1c3e6bd948db9a103328d94ad2c9a94.nq.gz
    ├── 3d4d11bf08038d60f84be00ff587ec233a54db62.nq.gz
    ├── 3e8137d58be9609a1e06ab04567d6a1ee3457f91.nq.gz
    ├── 3eabca41bb2c1437763f2ed5db06e705f9232bfb.nq.gz
    ├── 3f06748ea31d0847092e906f9c1800c4eff7e30b.nq.gz
    ├── 3fa9a3067dfde6785998cc5c1ca0006b1c1a6954.nq.gz
    ├── 3fcde910f589d74b4bf3678ee922c4efd94ffa1c.nq.gz
    ├── 43103733cd184e449d39d71a1ec54caa34997106.nq.gz
    ├── 43684c6fb80f16e4d8f3c81802d54bf36aa843f5.nq.gz
    ├── 454d1a3745ae95c57726af7a6ed3011050709c67.nq.gz
    ├── 455c794a55ba9feff235ae14e93e0c3260cdbcee.nq.gz
    ├── 45c6e6719e80040b7e6321953700642750655e51.nq.gz
    ├── 467a1d555689dc899fee898df0803bfebc2e7cfc.nq.gz
    ├── 474803eadab89b7a5ac01df674edbf1d04f43937.nq.gz
    ├── 47879f451cc5f7a5af0467c67ec6c209dfd5eb19.nq.gz
    ├── 49d8213977e8bbaec28f3c7421df175e13938f23.nq.gz
    ├── 4a09deb2b6ca082fbb203cfff5032bc0b972f4b9.nq.gz
    ├── 4b94ae3d9cfbcee799447ad6cb70a700dd934ff9.nq.gz
    ├── 4c3f14b624b168eafc8cd72beed7f2342cfbf027.nq.gz
    ├── 4dcf4d0855dfe46124040be66e2f77806fbfdcd0.nq.gz
    ├── 4e52578c4fd4218270d07e890daf5152e7ef5139.nq.gz
    ├── 4ee9ceef43586c3723aac8d45fb887a9046cd5b5.nq.gz
    ├── 506d06d495d79684e8b0d7801fc31402b09bc8c2.nq.gz
    ├── 50de0525629db7291adc8aecbab5b449230a26cb.nq.gz
    ├── 515f88a7a77a04c5ca49a8e90af68045e8876386.nq.gz
    ├── 5191f9cb80b4e7b2fe8a4f59e074ad343448f69a.nq.gz
    ├── 51eb7c4efb8badb3d465d9cc843c1f7f4ce416ac.nq.gz
    ├── 52e110bd4b368b031cf41a34e6d2aca878a396f6.nq.gz
    ├── 52f3626cef0b59fc4cc62166fc3478e989b34335.nq.gz
    ├── 5382f9bd246bac82c27f3a38821db3ec0a024a42.nq.gz
    ├── 53f7240dd12e5e299d769826c7c8172f82dfc758.nq.gz
    ├── 564042f6bd188a9c9a164db03b78af323fdcc845.nq.gz
    ├── 56d7029f77c5d721bb61f422f30a689da44a8d40.nq.gz
    ├── 56e4b0228be390031171f0cc676031792a0fac59.nq.gz
    ├── 5863ba39977003f9f574fe2aa3e1ab1382a14974.nq.gz
    ├── 5998fe7ad44cc0a340db66bdf326190007546419.nq.gz
    ├── 5a2f971e828e564ebc3fc57c5ccf15ebecd356e7.nq.gz
    ├── 5a416aa0a1fd8ee855dc6446f25e22d46f56880f.nq.gz
    ├── 5b637777e7c89fcb2d6af6ab11d344505cfd99a3.nq.gz
    ├── 5b913884cabbbd9764da768a626781f7bad1dee3.nq.gz
    ├── 5c13d84b2f8f797fa04379b09ac465275524f67d.nq.gz
    ├── 5c44e46aac64d26c30f4c7b90e925192a6b21393.nq.gz
    ├── 5db0351ee15fc421e2892e5235d6c6445420a450.nq.gz
    ├── 5f1a59bc79bfb8268731f4e74527be926bf60017.nq.gz
    ├── 62e4703d87efa7bd785c75d00a26d34454f3b87e.nq.gz
    ├── 64d35b4060a48dfb413fbd942503df591e70e1f9.nq.gz
    ├── 64ecefddbbcfa32c2d6e209ff9d150804ec9d6ff.nq.gz
    ├── 64f1b3f09c8003d59657a52b47fa366b45f3ea18.nq.gz
    ├── 6717b7d67996d84dbfe25f13e0306dbaeed45002.nq.gz
    ├── 6849c2211c4e76b43006ebcb7c800990c0942c97.nq.gz
    ├── 699a03d0e1cf0807e40854c54dcd6d809084e2da.nq.gz
    ├── 6a9a95fc447578d397f0cbd79415d98e807fa861.nq.gz
    ├── 6ab2d3615b1cc5a24b1ca41b0049c50e6abe1a7c.nq.gz
    ├── 6b27ea7bf26cf5c6ffe3fd559c999950681f3f32.nq.gz
    ├── 6bf16479ea3842603830affc0afa11d30753c541.nq.gz
    ├── 6d2dd72091cedca43b9205f770df1c2ad14e8377.nq.gz
    ├── 6e3c3d897aaee6d8e1139699a73523dcae827cd5.nq.gz
    ├── 702b4a20a5954b3ea9e9b36a983b120b4e244324.nq.gz
    ├── 71f669853a7fcb2518ef80ab55b12a3559191523.nq.gz
    ├── 73f9952b2407aa91111ba2440846c2112a98432e.nq.gz
    ├── 747468e84b24a34e64a1361a1d4527095ac06707.nq.gz
    ├── 752ab29a3477c010d40e0628896b71d6bd68e0a1.nq.gz
    ├── 7551c45a74d59532226744b4c8642307e3e739ae.nq.gz
    ├── 75a461d03857c190adbfc702bde5d9d2517287b5.nq.gz
    ├── 78076c5c109bf1a2cff330c8d4f7fc560609cadb.nq.gz
    ├── 797ccb2b0a340bbe889d03d3653a3b4e7d362e72.nq.gz
    ├── 7a8ffa228aff799cd5396263f32425960d46d743.nq.gz
    ├── 7d78c4972b772ca13746eeedf7e746d53a157310.nq.gz
    ├── 7e04f93ffd8c22fde55b49d7b1222406c4bbc37d.nq.gz
    ├── 7e5c69f1ac53be2e44bdfa8292f4d1ec44ef7322.nq.gz
    ├── 7f8e73c4be4a424a4510e8eae34c700737b04453.nq.gz
    ├── 7faed55d8e90a00b6fb21dfc7be4b45e6df7cc04.nq.gz
    ├── 805f5289911b3f462c0b55d6cc78d905ad539b0c.nq.gz
    ├── 80a7e11050324f14acc0488ea90f5d76360d4bd8.nq.gz
    ├── 80da415287440ffd12c274c741102e15f79ca02c.nq.gz
    ├── 811043bfbba311cb97473468bec424fe3c341320.nq.gz
    ├── 84bf4484ccbb3dbfa7f60389ba9f3edffebceebe.nq.gz
    ├── 87b25e09d1df52c6ae2db2a7ed63553c1ca66e21.nq.gz
    ├── 882fb8bd841d8e6d8c112d63d5c9239dd0d9619b.nq.gz
    ├── 895000398c2d034b2d0524a32f6b532a6896b7e0.nq.gz
    ├── 896a752115b596ca295533f01e9ea5bea6dace06.nq.gz
    ├── 899216898c8bde3671cd514e720436b08119792b.nq.gz
    ├── 89a4450fc406e5a638f6c4277ca2833ac37e0964.nq.gz
    ├── 8b41969398d71f9bcf4264ccbd89cd27ac35a772.nq.gz
    ├── 8ba3f00519d70b06469887790785dd0106d7bb2d.nq.gz
    ├── 8ce3dbc27d5a8455b563aac7c094915570f595bf.nq.gz
    ├── 8d930c21192c64777700c3d651942555838ea77f.nq.gz
    ├── 8ecd31329693357ef830c7e5eed85ad9e5d9ed61.nq.gz
    ├── 8fd9846ba77935f9718844d24d9b8b31b804853d.nq.gz
    ├── 92091239982cebd4975f9031459dc6024fb96493.nq.gz
    ├── 94a6d4222c4dec59e1102bfe2cb815a29658984d.nq.gz
    ├── 95ab805be7fe46aa83bd9befd36b373e8926369a.nq.gz
    ├── 962a6dbd3204892c84ba46180b6a7d229458b646.nq.gz
    ├── 964c711d30f5386a98bcccc2e47dbac969860d30.nq.gz
    ├── 99de57aa32f0e40f0a266ca0e84dbe8898e92fc9.nq.gz
    ├── 9a9e90ab36def2df4c20777fa9ec2c441cb347f7.nq.gz
    ├── 9c13794df6523f190c0c1e1d01a9c437353da521.nq.gz
    ├── 9c27584d794b7cc405f74cf3052dab1e52594bc2.nq.gz
    ├── 9d7aecc05bfad2d0c2f191733a414c118c8033e6.nq.gz
    ├── 9e0b1f334e5c5d953ba6e268464512de219cd44a.nq.gz
    ├── 9e2ed882746e1d4c8fd95f247afff9459b2fa8a4.nq.gz
    ├── a024b35e598f392c180b43f0e95de477351f1cf3.nq.gz
    ├── a0cc2e51ab600723cbb4f2b0013278135d983d32.nq.gz
    ├── a12054d52dd7dfc2005a0b28cd2007b96a7145f3.nq.gz
    ├── a4f9f80f1791cd801e7918bab90745b6f025775f.nq.gz
    ├── a5de8beca733bbb8d510e2b823cff7b9cb1cf6f3.nq.gz
    ├── a64e84fb5b52d8cbb179ca1270be848cf4bce557.nq.gz
    ├── a8b5b3f492dd2d7d946737710348e880c76644d4.nq.gz
    ├── aa6a127f4b58ca85c973a92e5f494c611f02e0b3.nq.gz
    ├── aaec84f13ec52dac78d638ca322820851615fbd4.nq.gz
    ├── ac99a5c735da9333b7163ec7700bac6a290881ef.nq.gz
    ├── ad1f736652d190fc5879417a0d11630bc3330671.nq.gz
    ├── ae5e3e19c55ce599c7de51dece39da559ca504e6.nq.gz
    ├── af0e8920b3adee483fbccbb87519fa5b88f3fd20.nq.gz
    ├── af503962641c3b210a96a34aac72b9d0a805df28.nq.gz
    ├── afdc12b253859580176f052ab0dea68b88d3f690.nq.gz
    ├── b1207d2d190e88cba6eccd7b6d5386d9fae3766c.nq.gz
    ├── b2b9be9c511ce49aab8eb924f173fefa0a99ed54.nq.gz
    ├── b324da3ff3d23daf003c1f1dd242b6657f496031.nq.gz
    ├── b3ff80c942bcf2f2a03492d693aa2d25f646709f.nq.gz
    ├── b4685aa65fd991cad75c02300173007eec4131eb.nq.gz
    ├── b4a3ed4359d91ebfb9db13c60a9a2d9d8b921f48.nq.gz
    ├── b59e80d1620adf0971282e618333719b9ca75750.nq.gz
    ├── b5e469c60081bd8a28c83ed762bbc8d230890ee8.nq.gz
    ├── b63c2803a6bfc8b10d7c85a4ad09cdef5d7ef70e.nq.gz
    ├── b6dfad87e231a71f5f5d5e925988da4d34df2e27.nq.gz
    ├── b6f53e2872efc3cca0986328f95265354f689c76.nq.gz
    ├── b789ec14019c644d1b011d0e0aaaef22e09e39bb.nq.gz
    ├── b8729725b161bf29836fa8ff211e202e2f7bf230.nq.gz
    ├── b9be9c7671a56a5ff26394de86475cde67f7252c.nq.gz
    ├── bc573929ebf390822f897603c8fe188c3ee1870e.nq.gz
    ├── bf6b773dd425cfb403393bbd3961bb0253a9e1d4.nq.gz
    ├── bfee539c13a0842533f0c74b905f035e33ca8f5c.nq.gz
    ├── c07f4527e1e78430de8360b967ca857721d4b910.nq.gz
    ├── c0f06279f7296d35d120d959b73c9fd2d3549d51.nq.gz
    ├── c314cef18aedb93349f4f881b2b48b5454274b48.nq.gz
    ├── c588847e8b84c21190da1d9832c512479e60acbe.nq.gz
    ├── c5cc703e24ad827bb397c379a189375e4a745ffa.nq.gz
    ├── c6b193deb8cbafc6708bba8f2c5a5e499fe4440b.nq.gz
    ├── c721d1064b21fe0012d62a493163186d13a39fd4.nq.gz
    ├── ca0fcbe68a4bc6cf233723effd1b1ab5eebdff0e.nq.gz
    ├── ca4683e25d513f9c1bdfb36b929206e406831531.nq.gz
    ├── caf0264047c21bbbab363e2d50c09ec604136e6a.nq.gz
    ├── ccb8e7ee17fd04cac07f32d4574fb941057a64f3.nq.gz
    ├── ccd9f2ead98e5e883e010d42dc39aaaa5bac8a6a.nq.gz
    ├── cd3c35fd47422667e4ea2948e970d84a33ccd4b8.nq.gz
    ├── cde36c91f9290c9dfe9f086e8a4f1dad8898ca09.nq.gz
    ├── d1020d0c4c234212248f77c4d83833e6a1a55896.nq.gz
    ├── d1cc958de645d843f660f203477c4fdc8f188e79.nq.gz
    ├── d31e272fec23a99d979afdfb9f2c0df160dc01e5.nq.gz
    ├── d892a6a9c0c497e0b683aa5507b4f4576d1f4fd8.nq.gz
    └── d8cd1984d4ac4d7a42b9ee42dac8f7234e1e3be8.nq.gz

11 directories, 200 files
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
*Parsed on 2026-09-24 by [repolex](https://repolex.ai)*
