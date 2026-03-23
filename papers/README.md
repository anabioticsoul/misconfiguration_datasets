# Misconfiguration Troubleshooting Papers

This directory contains the replication materials for the **misconfiguration troubleshooting papers** collected and analyzed in our literature review.

The current structure is organized by review stage:

- [filtering/](#Filtering-process): intermediate results produced during the paper search and screening process
- [agreement/](#Agreement-formation): annotation agreement files used to evaluate screening and labeling consistency
- [result/](#final-result): the final list of papers included in our review
  
## Overview

### Filtering process

This directory contains the intermediate artifacts generated during the paper collection and screening process. These files record how candidate studies were progressively identified, filtered, complemented, and refined before obtaining the final set of primary studies.

The current files include:

- `00_raw_papers.csv`: the initial set of retrieved candidate papers
- `01_filtering_keyword.csv`: the keyword-based screening results
- `02_snowballing.csv`: the papers collected through backward and/or forward snowballing
- `03_complement.csv`: the additional complementary papers collected during the review process

- 
### Agreement formation

This directory contains the files used for inter-rater agreement analysis. These materials are provided to improve the transparency of the manual screening and labeling process and to support the reproducibility of the literature review procedure.

The current files include:

- `paper_labels_for_kappa.csv`: the independent labels used for agreement calculation
- `paper_confusion_matrix.csv`: the confusion matrix generated from the independent screening results
- `final_kappa.log`: the log file recording the final agreement statistics

### Final result

The directory contains the final paper list used in our study.
  
## Paper Fields

The paper records in this directory may include the following fields:

- `ID`: the unique identifier assigned to each paper in our review
- `Title`: the title of the paper
- `Year`: the publication year of the paper
- `Acronym`: the acronym of the publication venue, journal, conference, workshop, or source

## Notes

- The screened papers in this directory are those considered relevant to **software misconfiguration troubleshooting** in the scope of our study.
