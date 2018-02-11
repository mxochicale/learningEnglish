fileinfo := LaTeX Makefile
author := Miguel P. Xochicale
version := alpha1

TEX = file
LATEX = pdflatex -shell-escape -interaction=nonstopmode -file-line-error
BIB = bibtex

all:
	$(LATEX) $(TEX).tex
	$(LATEX) $(TEX).tex
	#(BIB) $(TEX)
	# $(BIB) $(TEX)
	$(LATEX) $(TEX).tex
	$(LATEX) $(TEX).tex
	evince $(TEX).pdf &
	@echo "================================================"
	@echo "All done! pdf file has been created".
	@echo "================================================"

clean:
	rm -f *~
	rm -rf *.backup
	rm -f `ls $(TEX).* | grep -v .tex`
	echo "Cleaning complete!"



#rm -f `ls $(TEX).* | grep -v .tex | grep -v .pdf`
