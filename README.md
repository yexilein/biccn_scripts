
This directory contains R modules parsing the biccn data (synchronized with Github), and some RDS files containing parsed data (only locally).

# R modules

## Study specific modules
 - macosko_regev.R: functions used to parse the data from the Macosko_Regev subdirectory.
 - ecker.R: functions used to parse the data and metadata from the Ecker subdirectories
 - zeng.R: functions used to parse the data and metadata from the Zeng subdirectory.

## Fusion modules
 - fuse_datasets.R: functions used to create dataset mixing count data with metadata, as well as dataset covering multiple studies.


# RDS files

## Gene count matrices

All these files contain sparse matrices with gene counts, rownames are gene names and colnames are sample names.
 - ecker_atac_gene_counts.rds: ATACseq data from Ecker.
 - macosko_10x.rds: 10x nuclei from Macosko.
 - regev_10x.rds: 10x nuclei from Regev.
 - zeng_10x_cells.rds: 10x cells from Zeng.
 - zeng_smart_nuclei.rds: SMARTer nuclei from Zeng.

## Gene mapping

These files contain simple data frames mapping Ensembl IDs to gene names.
 - regev_mapping.rds: mapping based on Regev's GTF file.
 - sara_mapping.rds: mapping based on Sara's data.
