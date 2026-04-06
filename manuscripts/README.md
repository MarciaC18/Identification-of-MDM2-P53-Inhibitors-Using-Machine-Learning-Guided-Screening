# Manuscripts

This folder stores the manuscript sources associated with the broader `Marcia_MDMD2-P53` project. It is organized to hold multiple papers over time.

Current paper set:

- `MARCIAH_main.tex`: main application-note manuscript for the MARCIAH software workflow.
- `MARCIAH_SI.tex`: supporting information for the MARCIAH manuscript.
- `figures/q6_lie_schema.tex`: TikZ source for the workflow figure used in the main manuscript.
- `refs.bib`: bibliography shared by the current manuscript set.
- `submission_readiness.md`: submission and scope notes for the current draft.
- `word_count_statement.md`: approximate word-count note for the main manuscript.

Build locally from this folder with:

```bash
make
```

Or build each document separately with:

```bash
make main
make si
```
