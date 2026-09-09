# MLBioIGE

**M**achine **L**earning and **Bio**informatics to identify the **G**enetic **E**ffect of SARS-CoV-2 on idiopathic pulmonary fibrosis (IPF) patients.

People with idiopathic pulmonary fibrosis — long-term lung scarring — were hit especially hard by COVID-19. But *why*? What is happening at the gene level that makes SARS-CoV-2 infection more dangerous for IPF patients? This project answers that question by combining machine learning with bioinformatics.

## What was done

Using RNA-seq datasets from public gene expression repositories, the study:

1. **Ran differential expression analysis (DESeq2)** on COVID-19, COPD, and IPF datasets to find genes that behave differently in disease vs. healthy samples.
2. **Identified common genes** shared across conditions to uncover shared pathways and potential drug targets.
3. **Built protein–protein interaction (PPI) networks** to find hub genes and key functional modules.
4. **Mapped transcription factor–gene interactions** to understand the regulatory circuitry involved.

The result: a set of candidate genes, pathways, and drug targets explaining how SARS-CoV-2 infection compounds the complexity of IPF.

## Published paper

> Sk. Tanzir Mehedi, Kawsar Ahmed, Francis M. Bui, Musfikur Rahaman, Imran Hossain, Tareq Mahmud Tonmoy, Rakibul Alam Limon, Sobhy M. Ibrahim, Mohammad Ali Moni. "MLBioIGE: Integration and interplay of machine learning and bioinformatics to identify the genetic effect of SARS-CoV-2 on idiopathic pulmonary fibrosis patients." *Biology Methods and Protocols*, 2022.
> DOI: [10.1093/biomethods/bpac013](https://doi.org/10.1093/biomethods/bpac013)

## What's in this repo

| Folder | Contents |
|---|---|
| `paper/` | Published paper (Oxford Academic, 2022) and the final manuscript |
| `analysis/` | Final DESeq2 differential-expression notebooks — the consolidated analysis plus per-dataset versions for COVID-19 (GSE147507), COPD (GSE57148), and IPF (GSE52463) |
| `data/` | Filtered sample metadata for the three GEO datasets |

### Data note

The notebooks work with count matrices from GEO (GSE147507, GSE57148, GSE52463). The large count-data files are not stored here — download them from [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/) using the accession numbers above. Only the small sample-metadata files are included.

## Authors

Sk. Tanzir Mehedi, Kawsar Ahmed, Francis M. Bui, **Musfikur Rahaman**, Imran Hossain, Tareq Mahmud Tonmoy, Rakibul Alam Limon, Sobhy M. Ibrahim, Mohammad Ali Moni — University of Information Technology and Sciences (Dhaka), University of Saskatchewan, and collaborators.
