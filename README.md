# Marcia_MDMD2-P53

This repository contains the broader research material associated with the MDM2/p53 project. It is not the standalone software distribution for the MARCIAH workflow.

## Scope

The repository groups together project assets that support ongoing computational work, manuscript writing, and method development. The exact contents may evolve as the project grows, but the current structure includes:

- `manuscripts/` for paper drafts, supporting information, figures, and submission notes
- `Q6/`, `equilibration/`, and `protprep/` for project-specific setup and simulation material
- `Data/`, `Figures/`, and `Performance Metrics Calculations/` for analysis and reporting assets
- force-field and ligand-preparation files used during project development

## Manuscripts

The `manuscripts/` directory is designed to host multiple papers. The current manuscript set is centered on MARCIAH and includes:

- `manuscripts/MARCIAH_main.tex`
- `manuscripts/MARCIAH_SI.tex`

Build from that directory with:

```bash
cd manuscripts
make
```

## Software Repository

The executable MARCIAH workflow is maintained separately in the sibling repository:

```text
../MARCIAH
```

That repository contains the installable Conda environment, command-line setup script, CLI test script, and the cleaned execution example intended for external users and software testing.

## Separation of Roles

This repository keeps the paper sources and the broader project context. The MARCIAH repository keeps the reusable executable workflow that can be handed to a student or reviewer for installation and testing from scratch.
