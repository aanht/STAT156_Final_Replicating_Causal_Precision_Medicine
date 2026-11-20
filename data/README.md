# Data Descriptions

**TODO:** *to be further revised as we work on replicating the data summary stats (figure S3 & S4 pg. 22)*

**TODO:** *add descriptions for each column of each dataset that we used*

`pdxe_tissue.csv` (PATIENT_ID, Tissue): maps each tumor ID to its cancer tissue of origin (e.g., GC = gastric cancer, NSCLC = luncg cancer, BRCA, PDAC, CRC)

`pdxe_mut_and_cn2` (Sample, Gene, Category, Details): covariates table in long format; each row is one tumor + altered gene & a single tumor can have hundreds of mutated genes (Sample matches PATIENT_ID)
* To build the paper's dataset, we will filter this sheet for the four biomarkers used in the algorithm: KRAS, BRAF, PIK3CA, and PTEN.

`pct_raw_data`: raw day-by-day mouse tumor volume measurements (to be confirmed: most likely not needed since pct_curve_metrics has this summarized)

`pct_curve_metrics`: treatments ($K$) and outcomes ($Y$) table in long format; contains each tumor's response to each tested drug (binimetinib, BYL719, LEE011) ie. each row is one tumor + drug test

