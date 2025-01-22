

This repository examines the human cortical organoid single-cell RNA-seq dataset from Bhaduri et al. (2020).
Link to full text pdf: https://pmc.ncbi.nlm.nih.gov/articles/PMC7433012/

Install all relevant Bioconductor packages with:
```
BiocManager::install(remotes::local_package_deps(dependencies=TRUE))
```

### About the dataset
The data contains approximately 20,000 cells collected from the hippocampus, prefrontal (PFC), motor, parietal, somatosensory and V1 cortices. 
Individual cells were isolated using 10X Genomics droplet-based protocols and sequenced together on a NovaSeq S2 flow cell.
After sequencing, expression was quantified by counting the number of reads mapped to each gene (row) in each sample (column).
In theory, there is also cell-level metadata for this dataset but it could not be unambiguously mapped to the column names.
