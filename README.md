[![sihellem - ROA-UCE-DB](https://img.shields.io/static/v1?label=sihellem&message=ROA-UCE-DB&color=red&logo=github)](https://github.com/sihellem/ROA-UCE-DB "Go to GitHub repo")
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC_BY--NC--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![Generic badge](https://img.shields.io/badge/SystBiol-10.1093/sysbio/syae002-<COLOR>.svg)](https://doi.org/10.1093/sysbio/syae002)

# The Cockroach UCE Database
The Cockroach UCE Database. Centralization of cockroaches UCE data and assignation of unique identification code.

This database is maintained by the [Evolutionary Genomics Unit](https://groups.oist.jp/egu) at OIST.

For any question or request, please open an issue.

## A/ Referenced contributions of UCE data
Listed contributions to the [Database](roa_uce_db_ids.tsv).
| Contribution  | Number of samples | Reference | Data location |
| --------  | ------------------- | --------------------- | ------------------- |
| #1 | 61 | Kovacs _et al_. [_Syst Biol_](https://doi.org/10.1093/sysbio/syae002) | [_Dryad_](https://doi.org/10.5061/dryad.fxpnvx0wx) |

## B/ Methods and suggested database usage
For general documentation, refer to same section on the Termite UCE Database (TER-UCE-DB), at: [![sihellem - TER-UCE-DB](https://img.shields.io/static/v1?label=sihellem&message=TER-UCE-DB&color=red&logo=github)](https://github.com/sihellem/TER-UCE-DB#b-methods-and-suggested-database-usage "Go to GitHub repo")

Updated codes within each sub-section are provided below.

### B.1. Extraction of UCEs from newly-generated assemblies
The set of 319,243 baits targeting 30,059 UCE loci is available from _Dryad_ (File: [roaches-v1-master-probe-list-DUPE-SCREENED.fasta.gz](https://datadryad.org/stash/downloads/file_stream/2761879)).
This bait set was designed using six genomes:
- three publicly available genomes: _Blatella germanica_ (GenBank accession no. GCA_003018175.1), _Periplaneta americana_ (GCA_002939525.1), and the termite _Zootermopsis nevadensis_ (GCF_000696155.1);
- three in-house genomes: _Geoscapheus dilatatus_, _Neogeoscapheus hanni_, and _Panesthia cribrata_.

For details on the design, refer to the Supplementary Material on [Zenodo](https://zenodo.org/records/10398591).

```
### 1. Get the baits
## Dryad: roaches-v1-master-probe-list-DUPE-SCREENED.fasta.gz
wget https://datadryad.org/stash/downloads/file_stream/2761879 --output-document=roaches-v1-master-probe-list-DUPE-SCREENED.fasta.gz && gzip -d roaches-v1-master-probe-list-DUPE-SCREENED.fasta
```
### B.2. Leveraging the database
```
### 5. Generate the database
## Contribution #1
wget https://datadryad.org/stash/downloads/file_stream/2761883 --output-document=ROA_UCE_DB_CONTRIB_1.fasta.gz && gzip -d ROA_UCE_DB_CONTRIB_1.fasta.gz
```

## C/ How to cite
Kovacs, T.G.L, Walker, J., Hellemans, S., Bourguignon, T., Tatarnic, N.J., McRae, J.M., Ho, S.Y.W, Lo, N. 2024. Dating in the dark: elevated substitution rates in cave cockroaches (Blattodea: Nocticolidae) have negative impacts on molecular date estimates. _Systematic Biology_. doi: [10.1093/sysbio/syae002](https://doi.org/10.1093/sysbio/syae002)

[Preprint on _bioRxiv_ [2023.01.17.524483](https://doi.org/10.1101/2023.01.17.524483)]
