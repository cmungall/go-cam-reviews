# Executive Summary: GO-CAM Reviews of E3 Ubiquitin Ligases Models

The collected reviews provide a comprehensive assessment of various GO-CAM models describing E3 ubiquitin ligase pathways. Overall, most models correctly represent the activities and relationships of E3 ligases according to the best practice guide, though several common areas for improvement were identified:

1. **Most models correctly use appropriate molecular functions** (e.g., ubiquitin protein ligase activity GO:0061630, ubiquitin ligase-substrate adaptor activity GO:1990756)

2. **Common strengths** include proper causal relationships, cellular localization, and evidence annotations

3. **Common improvement areas** include:
   - More specific annotations for types of ubiquitination (e.g., K48-linked vs K63-linked)
   - Explicitly showing substrates using "has input" relationships
   - Complete representation of complexes when multiple components are involved
   - Consistent biological process annotations

## Detailed Examples

### Effective Implementation of E3 Ligase Guidelines

The model [gomodel:613aae0000000813](https://bioregistry.io/go.model:613aae0000000813) (Liver apoptosis regulation by CASP6) effectively represents how AMPK subunits negatively regulate CASP6 activity through phosphorylation, and how CASP6 activates BID through cleavage. The model correctly shows:

- CASP6 with cysteine-type endopeptidase activity (GO:0004197)
- Appropriate causal relationships with "directly positively regulates" (RO:0002629) and "directly negatively regulates" (RO:0002630)
- Clear biological context with hepatocyte apoptotic process (GO:0097284)

### Areas Needing Improvement

The model [gomodel:6246724f00000283](https://bioregistry.io/go.model:6246724f00000283) (Regulation of mTORC1 signaling via ubiquitination of SESN2) correctly shows RNF167 as an E3 ligase, but would benefit from:

- More explicit representation of the GATOR2 complex
- Clarifying the target of WDR24's ubiquitin ligase activity
- Better representing K63-linked ubiquitination specificity

The model [gomodel:6246724f00000369](https://bioregistry.io/go.model:6246724f00000369) (Regulation of mTORC1 via ubiquitination of CASTOR1) could be improved by:

- Adding specific lysine residues in CASTOR1 (K61, K96, K213) that are targets for K29-linked polyubiquitination
- Better representing how AKT1 phosphorylates CASTOR1 at Ser-14

### Exemplary Models

[gomodel:5ee8120100000947](https://bioregistry.io/go.model:5ee8120100000947) (SP-ANN-SEC14L1) effectively shows SEC14L1's protein sequestering activity correctly negatively regulating MAVS-RIG-I binding, demonstrating proper use of the guidelines for representing negative regulation through protein sequestration.

[gomodel:60ad85f700002694](https://bioregistry.io/go.model:60ad85f700002694) (TSLP-mediated signaling pathway) correctly implements the signaling receptor annotation guidelines, with proper ligand representation, receptor activities, and downstream effects.
