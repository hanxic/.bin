MAIN=main

all: $(MAIN).pdf

$(MAIN).pdf: $(MAIN).tex refs.bib
	latexmk --shell-escape -pdf $(MAIN)
	open $(MAIN).pdf

fast: $(MAIN).tex
	pdflatex $(MAIN)

clean:
	latexmk -C $(MAIN)
	rm -rf $(MAIN).pdf
