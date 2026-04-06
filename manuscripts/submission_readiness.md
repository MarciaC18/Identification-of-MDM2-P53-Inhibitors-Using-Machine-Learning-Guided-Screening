# MARCIAH Submission Readiness

This draft is aligned to the JCIM Application Note framing for the repository:

- `MARCIAH`

This draft is aligned to the JCIM Application Note framing:

- The application name appears in the title.
- The manuscript is written as a software/application note rather than as a full methods paper.
- It includes at least one figure.
- It contains dedicated `Data and Software Availability`, `Associated Content`, `Author Information`, and `Acknowledgments` sections, consistent with ACS article structure.
- The workflow advances are framed in terms of usability, automation, reproducibility, and reviewer testability.

Items still to finalize before submission:

- Confirm the final corresponding author choice and email if it should differ from the current manuscript header.
- Deposit the code in a public versioned repository and archive a release DOI.
- Confirm the intended supported operating systems with explicit tests.
- Add a short reviewer walkthrough for one ligand and one complex execution path once the public repository structure is frozen.
- Decide whether to keep the manuscript as an application note centered on workflow integration or expand it with a larger benchmark series.

Current source basis for technical claims:

- `../../MARCIAH/README.md`
- `../../MARCIAH/ligands/README.md`
- `../../MARCIAH/complex/README.md`
- Root analysis scripts in the target repository, including `analyze_LIE_noqgui.py`, `ligand-surrounding-energies.py`, `check_high_errors.py`, `prueba_2.py`, and `DG_regression_reference_ligands.py`

External journal/template basis used for this folder:

- Local `achemso` ACS manuscript class (`jcisd8` journal option)
- JCIM Application Note editorial DOI: `10.1021/ci500685s`
- ACS general submission guidance as summarized in the manuscript structure
