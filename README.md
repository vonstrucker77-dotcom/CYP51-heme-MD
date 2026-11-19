CYP51-Heme-MD

A reproducible, heme-aware molecular dynamics workflow for studying inhibitors of Candida albicans lanosterol 14α-demethylase (CYP51).

Research Objective

Compare ketoconazole and designed analogues in the CYP51 binding site while preserving the important interaction between the azole nitrogen and heme iron.

The long-term goal is to investigate whether structural modifications can retain antifungal activity while improving selectivity over human cytochrome P450 enzymes.

Target Structure

- Target: Candida albicans CYP51
- Reference structure: PDB 5TZ1
- Cofactor: Heme
- Main focus: Heme–azole coordination and ligand-binding stability.

Scientific Requirements

Production molecular dynamics must not begin until the heme model has been validated.

The workflow must establish:

1. Heme identity, oxidation state and coordination.
2. Appropriate heme force-field parameters and their scientific sources.
3. Correct treatment of protein–heme and ligand–iron interactions.
4. Structural validation after system preparation.
5. Successful minimization and equilibration.

A platform accepting a heme file does not automatically mean that its iron coordination is correctly modelled.

Planned Repository Structure

- "docs/" — Scientific rationale and protocols.
- "inputs/" — Receptor and ligand input documentation.
- "parameters/" — Validated heme and force-field parameters.
- "scripts/" — Preparation and simulation scripts.
- "results/" — Simulation and analysis outputs.

Current Progress

- [x] Public GitHub repository created.
- [x] Repository renamed to CYP51-Heme-MD.
- [x] Initial research scope established.
- [ ] Verify receptor structure and heme contents.
- [ ] Validate ligand structures and stereochemistry.
- [ ] Select and validate heme parameters.
- [ ] Prepare and validate the CYP51–ligand complex.
- [ ] Perform molecular dynamics simulations.
- [ ] Analyze structural stability and binding interactions.

Scientific Principle

A plausible molecular dynamics trajectory is not automatically a scientifically valid simulation.

Every preparation choice affecting the heme–azole interaction must be justified, documented and validated.
