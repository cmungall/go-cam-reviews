Based on my review of the GO-CAM model "gomodel:5fadbcf000000317" titled "Fzd3 function in Cranial neural crest cells" and the available documentation, I can provide the following assessment:

# GO-CAM Model Review: Fzd3 function in Cranial neural crest cells

**Model ID**: [gomodel:5fadbcf000000317](https://bioregistry.io/go.model:5fadbcf000000317)  
**Title**: Fzd3 function in Cranial neural crest cells  
**Taxon**: Xenopus laevis (African clawed frog) - NCBITaxon:8364

## Overall Assessment

This model describes the function of Frizzled-3 (Fzd3) in cranial neural crest cells in Xenopus, focusing on both canonical and non-canonical Wnt signaling pathways and their downstream effects on neural crest cell migration and development.

## Strengths

1. **Comprehensive representation**: The model captures both canonical and non-canonical Wnt signaling through Fzd receptors (Fzd3 and Fzd7).

2. **Cellular localization**: The model appropriately annotates subcellular locations for the activities (e.g., extracellular space for secreted Wnt proteins, plasma membrane for transmembrane receptors).

3. **Pathway connectivity**: The model shows a good flow of signaling from extracellular Wnt ligands through receptors to downstream effectors including RhoA, Rac1, JNK, and Rock1.

4. **Evidence support**: Most activities and relationships have supporting evidence with appropriate ECO codes and references to literature or databases.

## Areas for Improvement

1. **Obsolete term usage**: The model uses GO:1904929 "obsolete coreceptor activity involved in Wnt signaling pathway, planar cell polarity pathway" for PTK7.L. This term should be replaced with an up-to-date GO term.

2. **Incomplete evidence**: Some causal associations lack evidence codes, for example:
   - The causal association between Dvl1 (GO:0005109) and Fzd7 (GO:0042813)
   - The causal association between Wnt11 (GO:0005109) and Fzd7 (GO:0042813)
   - The causal association between Sdc4 (GO:0005515) and Fzd7 (GO:0042813)

3. **Signaling receptor representation**: According to the signaling receptor annotation guidelines, the input of a receptor should be the effector protein it regulates, not its ligand. However, in this model, the causal relationship between ligands and receptors is represented using "directly positively regulates" (RO:0002629) or "causally upstream of, positive effect" (RO:0002304).

4. **Missing biological process context**: Some molecular functions lack biological process context through "part of" relations, which would help situate the activities in their appropriate biological processes.

## Specific Recommendations

1. **Replace obsolete term**: Update GO:1904929 with an appropriate current term for PTK7's role in PCP signaling.

2. **Add missing evidence**: Add appropriate evidence codes and references for all causal associations that currently lack them.

3. **Clarify receptor-ligand relationships**: Consider whether the current representation of receptor-ligand relationships aligns with the "Signaling receptor activity annotation guidelines" document. The guideline states that a receptor's input should be its effector protein, not its ligand.

4. **Add biological process annotations**: For activities that lack them, consider adding "part of" relations to appropriate biological processes to provide better context.

5. **Check RhoA/JNK pathway**: Ensure that the pathway from RhoA to JNK aligns with current understanding. Typically, RhoA acts through ROCK to affect cytoskeletal dynamics, while JNK is often downstream of Rac1/Cdc42 in separate pathway branches.

## Biological Accuracy

The model appears to be biologically accurate based on the literature about Fzd3's role in neural crest cell development and migration in Xenopus. The key publications referenced in the model (PMID: 28427856, PMID: 11585792) support the signaling pathways depicted. The model correctly captures the relationships between Wnt signaling (both canonical and non-canonical pathways) and neural crest cell migration.

## Conclusion

This is a well-constructed GO-CAM model that effectively represents Fzd3 function in cranial neural crest cells in Xenopus, with a few areas that could be improved for completeness and alignment with current GO-CAM curation guidelines. The model provides a valuable resource for understanding the molecular mechanisms underlying neural crest development.