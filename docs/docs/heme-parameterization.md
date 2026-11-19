Heme Parameterization Strategy

1. Scientific Background

Candida albicans CYP51 contains a heme prosthetic group with an iron centre.

Azole antifungal drugs inhibit CYP51 by coordinating one of their ring nitrogen atoms to the heme iron.

This interaction is essential to the binding mechanism and must be preserved during molecular dynamics simulations.

2. Candidate Force Field

The initial candidate is an AMBER-based workflow.

Proposed components:

- Protein: AMBER ff14SB
- Small molecules: GAFF
- Heme: Shahrokh et al. (2012) AMBER-compatible parameters
- Solvent: TIP3P water

Reference:

Shahrokh K, Orendt A, Yost GS, Cheatham TE III. (2012).

Quantum mechanically derived AMBER-compatible heme parameters for various states of the cytochrome P450 catalytic cycle.

DOI: 10.1002/jcc.21922

3. CYP51-Specific Considerations

The azole nitrogen coordinates with the heme iron as the sixth axial ligand.

The heme model must therefore represent:

1. Four porphyrin nitrogen–iron interactions.
2. The proximal cysteine sulfur–iron interaction.
3. The distal azole nitrogen–iron interaction.
4. The appropriate iron oxidation and spin state.

4. Validation Requirements

Before production MD:

- Confirm heme atom identities and connectivity.
- Confirm iron oxidation and spin-state assumptions.
- Verify the Fe–S and Fe–N coordination model.
- Check heme geometry against the experimental structure.
- Check that the azole remains coordinated to iron during minimization.
- Inspect energy stability during equilibration.

5. Important References

1. Shahrokh et al. (2012). DOI: 10.1002/jcc.21922.
2. Molecular Dynamics Investigations of Binding Mechanism for Triazoles Inhibitors to CYP51 (2020). DOI: 10.3389/fmolb.2020.586540.
3. Oda et al. (2005). DOI: 10.1002/jcc.20221.

6. Current Status

The AMBER-based approach is a candidate protocol, not yet a validated CYP51-heme model.

Further verification of the axial azole–iron coordination parameters is required before simulation.
