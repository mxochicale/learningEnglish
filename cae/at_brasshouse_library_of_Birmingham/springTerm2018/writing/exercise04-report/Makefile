fileinfo := LaTeX Makefile
author := Miguel P. Xochicale
version := alpha1

#filetex = file
LATEX = pdflatex -shell-escape -interaction=nonstopmode -file-line-error
BIB = bibtex

all:
	$(LATEX) $(filetex).tex
	$(LATEX) $(filetex).tex
	#(BIB) $(filetex)
	# $(BIB) $(filetex)
	$(LATEX) $(filetex).tex
	$(LATEX) $(filetex).tex
	evince $(filetex).pdf &
	@echo "================================================"
	@echo "All done! pdf file has been created".
	@echo "================================================"

clean:
	rm -f *~ *.log .log
	rm -rf *.backup
	rm -f `ls $(filetex).* | grep -v .tex`
	echo "Cleaning complete!"



#rm -f `ls $(filetex).* | grep -v .tex | grep -v .pdf`
