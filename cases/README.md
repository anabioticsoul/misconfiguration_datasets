# Misconfiguration Cases

This directory contains the replication materials for the **real-world misconfiguration cases** used in our study.

The current structure is organized by analysis stage:
- [filtering/](#Filtering-process): intermediate results produced during the case collection and filtering process
- [classification/](#classification): the final classified case dataset and related classification results
- [agreement/](#Agreement-formation): annotation agreement files used to evaluate labeling consistency

## Overview

### Filtering process

This directory contains the intermediate artifacts generated during the case selection process.

These files record how candidate cases were filtered and refined before obtaining the final set of real-world misconfiguration cases.

### Classification

This directory contains the final classified dataset of misconfiguration cases.

The classified cases include root-cause labels based on our revised taxonomy.  
Each case record is associated with a root-cause category and a more fine-grained subtype.

The four high-level root-cause categories are:

- `CA`: Constraint violation
- `CB`: Resource unavailability
- `CC`: Component-dependency error
- `CD`: Configuration semantic misinterpretation

The corresponding subtypes include:

- **Constraint violation**: _syntax error_, _invalid name_, _misplaced configuration_, _duplicate option_, and _multi-configuration error_
- **Resource unavailability**: _resource identifier mismatch_, _resource competition_, _unauthorized resource access_, and _hardware limitation_
- **Component-dependency error**: _component incompatibility_, _component missing_, and _cross-component misconfiguration_
- **Configuration semantic misinterpretation**: _ambiguous option name_, and _option value and functional requirement mismatch_

### Agreement formation

This directory contains the files used for inter-rater agreement analysis.

These materials are provided to improve the transparency of the manual annotation process and to support the reproducibility of the case-labeling procedure.

## Case Fields

The case records in this directory may include the following fields:

- `ID`: the case identifier
- `Software`: the target software system
- `Link`: the URL of the original discussion thread or issue report
- `Description`: a brief summary of the misconfiguration case
- `Subtype`: the fine-grained root-cause subtype assigned to the case
- `Year`: the year when the configuration-related issue was raised
- `Last Modified`: the last recorded modification time of the original source

## Notes

- The prefix of `ID` indicates the corresponding high-level root-cause category.
- The terminology in this directory follows the revised taxonomy used in the current version of the study.
