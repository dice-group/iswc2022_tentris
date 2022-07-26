This page provides access to all the scripts, data and code needed to reproduce the results of the paper:

> Alexander Bigerl, Lixi Conrads, Charlotte Behning, Muhammad Saleem and Axel-Cyrille Ngonga Ngomo (2022) Hashing the
> Hypertrie: Space- and Time-Efficient Indexing for SPARQL in Tensors. In: The Semantic Web – ISWC 2022
> Hashing the Hypertrie: Space- and Time-Efficient Indexing for SPARQL in Tensors

Cite as:

```
@InProceedings{bigerl2022hashing-the-hypertrie,
  author = {Bigerl, Alexander and Conrads, Lixi and Behning, Charlotte and Sherif, Mohamed Ahmed and Saleem, Muhammad and Ngonga Ngomo, Axel-Cyrille},
  booktitle = {The Semantic Web -- ISWC 2022},
  publisher = {Springer International Publishing},
  title = { {H}ashing the {H}ypertrie: {S}pace- and {T}ime-{E}fficient {I}ndexing for {SPARQL} in {T}ensors},
  url = {https://papers.dice-research.org/2022/ISWC_Hashing_the_Hypertrie/iswc2022_hashing_the_hypertrie_public.pdf},
  year = 2022
}
```

## Abstract

Time-efficient solutions for querying RDF knowledge graphs depend on indexing structures with low response times to
answer SPARQL queries rapidly. Hypertries—an indexing structure recently developed for tensor-based triple stores—have
achieved significant runtime improvements over several mainstream storage solutions for RDF knowledge graphs. However,
the space footprint of this novel data structure is still often larger than that of many mainstream solutions. In this
work, we detail means to reduce the memory footprint of hypertries and thereby further speed up query processing in
hypertrie-based RDF storage solutions. Our approach relies on three strategies: (1) the elimination of duplicate nodes
via hashing, (2) the compression of non-branching paths, and (3) the storage of single-entry leaf nodes in their parent
nodes. We evaluate these strategies by comparing them with baseline hypertries as well as popular triple stores such as
Virtuoso, Fuseki, GraphDB, Blazegraph and gStore. We rely on four datasets/benchmark generators in our evaluation: SWDF,
DBpedia, WatDiv, and WikiData. Our results suggest that our modifications significantly reduce the memory footprint of
hypertries by up to 70% while leading to a relative improvement of up to 39% with respect to average Queries per Second
and up to 740% with respect to Query Mixes per Hour.

## Reproducing Evaluation

Source code for our systems: [hypertrie](https://github.com/dice-group/hypertrie/tree/iswc2022-hashing-the-hypertrie)
and [<span style="font-variant:small-caps;">Tentris</span>](https://github.com/dice-group/tentris/tree/1.1.2)

A Script to recreate the full experimental setup, including all datasets, queries, triple stores, configurations and
scripts to run the experiments is available
from [here](https://github.com/dice-group/tentris-paper-benchmarks/tree/v2.0).

The raw data and scripts for generating the images are available
from [here](https://github.com/dice-group/hashing-the-hypertrie-eval/tree/iswc2022-hashing-the-hypertrie).


