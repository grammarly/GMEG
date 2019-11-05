# Enabling Robust Grammatical Error Correction in New Domains: Data Sets, Metrics, and Analyses

```
@article{doi:10.1162/tacl_a_00282,
author = {Napoles, Courtney and Nădejde, Maria and Tetreault, Joel},
title = {Enabling Robust Grammatical Error Correction in New Domains: Data Sets, Metrics, and Analyses},
journal = {Transactions of the Association for Computational Linguistics},
volume = {7},
number = {},
pages = {551-566},
year = {2019},
doi = {10.1162/tacl_a_00282},
URL = {https://doi.org/10.1162/tacl_a_00282},
eprint = {https://doi.org/10.1162/tacl_a_00282},
abstract = { Until now, grammatical error correction (GEC) has been primarily evaluated on text written by non-native English speakers, with a focus on student essays. This paper enables GEC development on text written by native speakers by providing a new data set and metric. We present a multiple-reference test corpus for GEC that includes 4,000 sentences in two new domains (formal and informal writing by native English speakers) and 2,000 sentences from a diverse set of non-native student writing. We also collect human judgments of several GEC systems on this new test set and perform a meta-evaluation, assessing how reliable automatic metrics are across these domains. We find that commonly used GEC metrics have inconsistent performance across domains, and therefore we propose a new ensemble metric that is robust on all three domains of text.}
}
```

## Repository Contents

### Data
`data/` contains the dev and test splits, with a subdirectory for each domain
containing
* the original sentences (`source`)
* system outputs (`amu`, `lstm`, `lstm-r`, `marian`, `nus`, `transformer`)
* human corrections (`ref[0-3]`)
* negative control used for collecting human ratings (`source+error`)

Domains are `fce`, `wiki`, and `yahoo`.

`DOMAIN-corpus-scores.csv` has the mean human rating for each system for that domain.
`DOMAIN-segment-scores.csv` has the mean human rating by sentence for each system.

### Metric

Coming soon. Please watch this repository or email courtney.napoles@grammarly.com
for updates.
