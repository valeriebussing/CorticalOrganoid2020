

This repository examines a heterogeneous dataset from a study of cell types in the mouse brain [@zeisel2015brain].

Install all relevant Bioconductor packages with:

BiocManager::install(remotes::local_package_deps(dependencies=TRUE))
Building the book can be done by either running the usual bookdown invocation in inst/book:

bookdown::render_book("index.Rmd")
Or by R CMD build on the package itself to compile the book during the vignette build process.

## About the dataset
The data contains approximately 3000 cells of varying types such as oligodendrocytes, microglia and neurons. 
Individual cells were isolated using the Fluidigm C1 microfluidics system [@pollen2014lowcoverage] and library preparation was performed on each cell using a UMI-based protocol.
After sequencing, expression was quantified by counting the number of unique molecular identifiers (UMIs) mapped to each gene.
