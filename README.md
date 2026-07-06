# OntGQA Ontology Graph

This repository releases the ontology graph constructed for the ACL 2026 Main paper:

> **Reasoning with Ontology Graph: Toward Type-Constrained Knowledge Graph Question Answering**

At this stage, we only release the constructed ontology graph file. More code, scripts, and resources related to the paper will be released gradually.

## Released Resource

```text
ontology_graph_freebase.json
```

`ontology_graph_freebase.json` is the Freebase ontology graph constructed in our paper. It provides relation-centric type information for KGQA research, where relations are associated with head and tail entity types.

This resource can be useful for:

- type-constrained knowledge graph question answering;
- relation-path filtering and pruning;
- schema-aware candidate retrieval;
- ontology-guided multi-hop reasoning;
- research on Freebase schema and relation-type structures.

## Citation

If you use this ontology graph, please cite our paper:

```bibtex
@inproceedings{shan-etal-2026-reasoning,
    title = "Reasoning with Ontology Graph: Toward Type-Constrained Knowledge Graph Question Answering",
    author = "Shan, Yongxue  and
      Peng, Jie  and
      Dong, Zixuan  and
      Hu, Fei  and
      Wang, Xiaodong",
    editor = "Liakata, Maria  and
      Moreira, Viviane P.  and
      Zhang, Jiajun  and
      Jurgens, David",
    booktitle = "Proceedings of the 64th Annual Meeting of the {A}ssociation for {C}omputational {L}inguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2026",
    address = "San Diego, California, United States",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2026.acl-long.489/",
    doi = "10.18653/v1/2026.acl-long.489",
    pages = "10684--10697",
    ISBN = "979-8-89176-390-6",
    abstract = "Large language models (LLMs) have recently advanced knowledge graph question answering (KGQA), but current methods tend to rely on LLM-induced type systems with inconsistent granularity, or perform multi-hop reasoning without explicit target-type constraints. We introduce OntGQA, a type-constrained KGQA framework that reasons over a relation-centric ontology graph, where each relation is labeled with its head and tail entity types to provide a stable schema backbone. Built on this graph, OntGQA adopts a planner{--}judge architecture with generative backoff: a type planner proposes plausible head{--}tail type pairs, a judge verifies retrieved candidates and their paths, and a generator is invoked only when all candidates are rejected. By constraining both endpoints of reasoning in type space, OntGQA achieves state-of-the-art performance and produces ontology-grounded reasoning chains, with substantial Hit@1 gains (87.7{\%}{\textrightarrow}91.5{\%} on WebQSP and 67.6{\%}{\textrightarrow}74.6{\%} on CWQ)."
}
```
