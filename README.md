<img align="right" width="200" src="img/logo.png">

Helix SARS-CoV-2 Surveillance
=============================
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=%40my_helix)](https://twitter.com/my_helix)

Helix® is no longer updating this repository. However, the dashboards below are still being updated regularly.

[Helix COVID-19 Surveillance Dashboard](https://helix.com/covid19db)

This data is being made available via the [Creative Commons Attribution Share Alike license](https://creativecommons.org/licenses/by-sa/4.0/deed.en)

<p align="right">
<a href="https://creativecommons.org/licenses/by-sa/4.0/deed.en"><img src="https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg"></a>
</p>

## 📚 Datasets

### counts_by_state.csv 📃
- This file contains counts of test results aggregated by state and collection date.
- Records with fewer than 3 positives are removed to protect privacy.
- All records have a qPCR quantification cycle (Cq) of less than 27 for the N gene target.

| Column Name | Description |
|-------------|-------------|
| state | Patient state of residence |
| collection_date | Date of specimen collection |
| positive | Number of positive test results |
| all_SGTF | Number of positive test results with S gene target failure |
| sequenced_SGTF | Number of sequenced test results with S gene target failure |
| B117 | Number of positive test results that were sequenced and known to be of the B.1.1.7 lineage |

### sequencing_results.csv 📃
- This file contains metadata for individual sequenced specimens, including GenBank Accession numbers and other [GenBank](https://www.ncbi.nlm.nih.gov/labs/virus/vssi/#/virus?SeqType_s=Nucleotide&VirusLineage_ss=SARS-CoV-2,%20taxid:2697049) metadata to facilitate retrieval of the viral genome sequence data.
- Samples without GenBank Accession numbers have been sequenced but are not yet submitted to or approved by GenBank.

| Column Name | Description |
|-------------|-------------|
| STM_id | Specimen ID |
| GISAID_virus_name | [GISAID Virus Name](https://www.gisaid.org/) |
| sex | Patient sex |
| state | Patient state of residence |
| lineage | [Pangolin](https://github.com/cov-lineages/pangolin) assigned SARS-CoV-2 lineage |
| clade | [Nextclade](https://clades.nextstrain.org/) assigned SARS-CoV-2 clade |
| age_bracket | Patient's age bracket at time of specimen collection |
| ncbi_accession_id | [NCBI GenBank Accession ID](https://www.ncbi.nlm.nih.gov/labs/virus/vssi/#/virus?SeqType_s=Nucleotide&VirusLineage_ss=SARS-CoV-2,%20taxid:2697049) |
| extra | Additional GenBank identifiers |
| subname | GenBank subname |
| sequence_length | GenBank sequence length |
| createdate | GenBank record creation date (YYYY/MM/DD) |
| updatedate| GenBank record update date (YYYY/MM/DD) |
