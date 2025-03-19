Based on the information gathered, I'll now review the GO-CAM model "gomodel:62900b6400000022" - Mono-ADP-ribosylation of ribosome subunits by PARP16 (Human).

# GO-CAM Model Review: Mono-ADP-ribosylation of ribosome subunits by PARP16

## Model Overview

**Title**: Mono-ADP-ribosylation of ribosome subunits by PARP16 (Human)  
**ID**: [gomodel:62900b6400000022](https://bioregistry.io/go.model:62900b6400000022)  
**Taxon**: Human (NCBITaxon:9606)  
**Status**: Production

## Summary of Model Content

This model describes how PARP16 (Q8N5Y8) mono-ADP-ribosylates specific ribosomal subunits (RPS6/P62753 and RPL24/P83731) in a process that is supported by NMNAT2 (Q9BZQ4). The model shows this leads to negative regulation of cytoplasmic translation (GO:2000766).

The model depicts:
1. PARP16's NAD+-protein-glutamate ADP-ribosyltransferase activity (GO:0140807) directly negatively regulating (RO:0002630) the structural constituent of ribosome activity (GO:0003735) of both RPS6 and RPL24
2. NMNAT2's protein ADP-ribosyltransferase-substrate adaptor activity (GO:0140768) directly positively regulating (RO:0002629) PARP16's ADP-ribosyltransferase activity

## Review Assessment

### Biological Content Accuracy

The model accurately captures the biological process described in the literature. The PMID:34314702 paper ("Ribosome ADP-Ribosylation Inhibits Translation and Maintains Proteostasis in Cancers") clearly shows that:

1. PARP16 mono-ADP-ribosylates ribosomal proteins RPS6 (at Glu-35) and RPL24 (at Glu-4)
2. NMNAT2 supports this activity by providing NAD+ and acting as an adaptor protein
3. This modification inhibits translation by preventing proper ribosome assembly (via mechanisms involving eIF6)

The model correctly captures these key relationships, including the negative regulatory effect on translation.

### GO-CAM Best Practices Compliance

**Structure and Relationships**:
- The model follows GO-CAM best practices by using appropriate terms for molecular activities, linking them through standard causal relations
- Each activity is properly enabled by a specific gene product
- All molecular functions are correctly placed as part of a broader biological process (GO:2000766)

**Use of Relations**:
- The use of RO:0002630 (directly negatively regulates) correctly represents the inhibitory relationship between PARP16's ADP-ribosylation activity and the ribosomal protein's structural activity
- The use of RO:0002629 (directly positively regulates) correctly represents NMNAT2's adaptor role in enhancing PARP16 activity

**Cellular Context**:
- The model correctly specifies the cellular context of cytosolic ribosome (GO:0022626) for the ribosomal protein activities

**Evidence**:
- All claims are supported by appropriate experimental evidence codes (ECO:0000314 - direct assay evidence) from the publication PMID:34314702
- The contributor is identified with an ORCID

### Areas for Improvement

1. **Additional Cellular Context**: While the model shows the ribosomal proteins in the cytosolic ribosome, it doesn't specify the subcellular location for PARP16 and NMNAT2. According to UniProt and the paper, PARP16 is localized to the ER membrane, while NMNAT2 is associated with Golgi/cytoplasmic vesicles. Adding these locations would enhance the model.

2. **Representation of Mechanism Detail**: The model could benefit from additional details about how ADP-ribosylation inhibits translation, specifically the mechanism involving eIF6 binding to ribosomes that prevents 60S-40S subunit joining. This is a key finding in the paper.

3. **Transport Activity**: The paper mentions that NMNAT2 is delivered to the site of action via Golgi-derived cytoplasmic vesicles. This transport activity could be included in a more comprehensive model.

4. **Output of Activity**: The model could be expanded to show exactly what species of ADP-ribosylated proteins are produced (e.g., ADP-ribosyl glutamic acid modifications at specific sites - Glu-35 for RPS6 and Glu-4 for RPL24).

## Conclusion

The GO-CAM model "Mono-ADP-ribosylation of ribosome subunits by PARP16 (Human)" is a well-constructed representation of the biological process described in the literature. It accurately captures the key molecular activities and their causal relationships, using appropriate GO terms and relation ontology predicates.

The model effectively shows how PARP16 mono-ADP-ribosylates ribosomal proteins (RPS6 and RPL24) with support from NMNAT2, leading to negative regulation of cytoplasmic translation. All assertions are well-supported by experimental evidence from the publication.

While the model could be enhanced with additional details about subcellular locations and mechanistic details, it successfully represents the core biological process in accordance with GO-CAM standards and best practices.