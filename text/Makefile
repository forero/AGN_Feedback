LATEX = pdflatex
MAIN = blurb_ngc3783

main: $(MAIN).tex
	$(LATEX) $(MAIN).tex
	bibtex $(MAIN)
	$(LATEX) $(MAIN).tex
	$(LATEX) $(MAIN).tex

clean:
	rm -f $(MAIN).aux
	rm -f $(MAIN).log
	rm -f $(MAIN).blg
	rm -f $(MAIN).bbl
	rm -f *~

view:
	open $(MAIN).pdf &