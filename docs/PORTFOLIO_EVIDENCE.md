# Portfolio Evidence: Bedrock RAG Lab

## Scope and Provenance

This is Jyothesh Karnam's personal write-up of a guided [NextWork RAG lab](http://learn.nextwork.org/projects/ai-rag-bedrock). The learning exercise, tutorial assets and platform services should not be presented as an independently developed production application. Original tutorial branding and the lab PDF are retained.

## Inspectable Evidence

| Repository source | What it supports | Boundary |
|---|---|---|
| [README](../README.md) | Author's account of S3 ingestion, embeddings, retrieval, model troubleshooting and prompt experiments | Historical self-reported exercise; no independent runtime verification |
| [Architecture image](../architecture-complete.png) | Conceptual document/S3, knowledge-base chunking/embeddings, OpenSearch Serverless and model flow | High-level learning diagram; omits detailed identity, network and failure controls |
| [Lab PDF](../legendary-ai-rag-bedrock.pdf) | Retained supporting lab artifact | Not a deployment receipt or reproducible source package |

## Service Choices Described in the Lab

- **Amazon S3:** document source.
- **Amazon Bedrock Knowledge Bases:** ingestion, chunking and retrieval workflow.
- **Titan Text Embeddings v2:** embedding model named in the original notes.
- **Amazon OpenSearch Serverless:** vector store shown in the diagram and described in the notes.
- **Llama model through Bedrock:** response generation; the specific models mentioned are historical observations.

RAG supplies retrieved context to generation. It does not establish model training or a guarantee that responses use only those documents. The [AWS explanation](https://docs.aws.amazon.com/bedrock/latest/userguide/kb-how-it-works.html) distinguishes ingestion and retrieval from response generation.

## Limitations

There is no application source, infrastructure as code, pinned environment, automated evaluation suite, current live endpoint or cost measurement in this repository. No commands were executed against AWS to validate the historical exercise. More detailed answers and one out-of-scope refusal are qualitative observations, not accuracy or safety benchmarks.

A later reproducible version would need a permitted sample corpus, recorded configuration, question/reference set, retrieval and groundedness evaluation, access controls, failure behavior and resource cleanup guidance. Those are future improvements, not implemented features. Check current AWS access, regional availability and pricing before any new resource creation.
