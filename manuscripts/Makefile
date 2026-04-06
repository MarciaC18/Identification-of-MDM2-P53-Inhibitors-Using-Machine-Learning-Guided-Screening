TEX=pdflatex
BIBTEX=bibtex
MAIN=MARCIAH_main
SI=MARCIAH_SI
MAIN_PDF=$(MAIN).pdf
SI_PDF=$(SI).pdf
MAIN_TEXS=$(MAIN).tex figures/q6_lie_schema.tex refs.bib
SI_TEXS=$(SI).tex refs.bib

.PHONY: all main si bib clean distclean rebuild wordcount

all: main si

main: $(MAIN_PDF)

si: $(SI_PDF)

$(MAIN_PDF): $(MAIN_TEXS)
	$(TEX) -interaction=nonstopmode $(MAIN).tex
	$(BIBTEX) $(MAIN)
	$(TEX) -interaction=nonstopmode $(MAIN).tex
	$(TEX) -interaction=nonstopmode $(MAIN).tex

$(SI_PDF): $(SI_TEXS)
	$(TEX) -interaction=nonstopmode $(SI).tex
	$(TEX) -interaction=nonstopmode $(SI).tex
	$(TEX) -interaction=nonstopmode $(SI).tex

bib:
	$(BIBTEX) $(MAIN)

wordcount:
	texcount -inc -sum=1 $(MAIN).tex

clean:
	rm -f $(MAIN).aux $(MAIN).bbl $(MAIN).blg $(MAIN).log $(MAIN).out
	rm -f $(SI).aux $(SI).bbl $(SI).blg $(SI).log $(SI).out

distclean: clean
	rm -f $(MAIN_PDF) $(SI_PDF)

rebuild: distclean all
