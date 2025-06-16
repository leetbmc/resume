# Makefile to compile LaTeX resume with xelatex

TEXFILE = brendan_coffey_resume
PDFFILE = $(TEXFILE).pdf
HTMLFILE = $(TEXFILE).html

all: $(PDFFILE)
html: $(HTMLFILE)

$(PDFFILE): $(TEXFILE).tex
	xelatex -interaction=nonstopmode $(TEXFILE).tex
	xelatex -interaction=nonstopmode $(TEXFILE).tex  # Run twice for TOC/page refs

clean:
	rm -f *.aux *.log *.out *.toc *.lof *.lot *.nav *.snm *.fls *.fdb_latexmk
	rm -f $(PDFFILE)

distclean: clean
	rm -f $(PDFFILE)

.PHONY: all clean distclean
