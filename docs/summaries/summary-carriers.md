# Review of GO-CAM Models for Molecular Carriers

## Executive Summary

The review of various GO-CAM models representing molecular carriers reveals good adherence to best practices in most cases, with some areas for improvement. Many models correctly implement the guidelines by:

1. Using appropriate molecular carrier activity terms (GO:0140104)
2. Properly specifying inputs and outputs for carrier activities
3. Correctly connecting activities with appropriate causal relationships
4. Providing proper cellular localization

Common issues that appear across models include:
- Missing input/output annotations for some carrier molecules
- Inconsistent use of causal relations (using various predicates instead of "provides input for")
- Inadequate specification of carried molecules
- Incomplete biological process context

## Detailed Examples

### Good Implementation Examples

1. **TLR4 Signaling Pathway (gomodel:5f46c3b700001031)**
   - [Link to model](https://bioregistry.io/go.model:5f46c3b700001031)
   - Exemplary use of molecular carrier activity for LBP and CD14 carrying LPS
   - Correctly represents:
     - LBP and CD14 with molecular carrier activity (GO:0140104)
     - LPS (CHEBI:16412) properly annotated as both input and output
     - Appropriate "provides input for" (RO:0002413) causal relations
     - Proper localization in extracellular space

2. **TSLP Mediated Signaling Pathway (gomodel:6246724f00000763)**
   - [Link to model](https://bioregistry.io/go.model:6246724f00000763)
   - Correctly annotates TSLP with cytokine activity in extracellular space
   - Well-connected pathway from ligand to receptor to downstream effectors

### Areas for Improvement

1. **IL1beta Mediated Signaling Pathway (gomodel:59cc772c00000000)**
   - [Link to model](https://bioregistry.io/go.model:59cc772c00000000)
   - Missing input specifications: The CD14 and LBP molecular carrier activities don't explicitly show what they're carrying
   - Recommendation: Add IL-1β as input and output for the carrier activities

2. **Cobalamin Metabolic Process (gomodel:61283a3000000217)**
   - [Link to model](https://bioregistry.io/go.model:61283a3000000217)
   - Missing cellular components: MMADHC has molecular carrier activity but lacks proper cellular localization
   - Recommendation: Add specific localization information for all carrier activities

3. **Hyaluronan Biosynthetic Process (gomodel:6246724f00000443)**
   - [Link to model](https://bioregistry.io/go.model:6246724f00000443)
   - Missing input annotations: Abcc5 exports hyaluronic acid but lacks clear annotation of inputs
   - Recommendation: Add explicit has_input relationships for the transported molecules

## Recommendations for Improvement

Based on the review, curators should ensure:

1. **Complete input/output specification**: Each molecular carrier activity should explicitly identify what molecule is being carried using the has_input and has_output relations.

2. **Consistent causal relationships**: Use "provides input for" (RO:0002413) for connecting carrier activities to downstream activities in metabolic/transport pathways.

3. **Precise cellular localization**: Always specify where the carrier activity takes place using "occurs in" relations to cellular component terms.

4. **Biological process context**: Connect carrier activities to the appropriate biological processes they participate in using "part of" relations.

5. **Molecular specificity**: When appropriate, use specific CHEBI IDs or other identifiers for the carried molecules to enhance clarity and searchability.

These improvements would further strengthen the value of GO-CAM models representing molecular carrier activities, making them more complete and useful resources for understanding molecular transport mechanisms.
