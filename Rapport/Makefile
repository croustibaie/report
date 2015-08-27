NAME=Rapport

all: *.tex *.bib
	@echo "make clean"
	@make clean > /dev/null 2> /dev/null
	@echo "pdflatex $(NAME).tex"
	@pdflatex $(NAME).tex >/dev/null 2> /dev/null
	@echo "bibtex $(NAME).aux"
	@bibtex $(NAME).aux >/dev/null 2> /dev/null
	@echo "makeglossaries $(NAME).glo"
	@makeglossaries $(NAME).glo >/dev/null 2> /dev/null
	@echo "makeindex $(NAME).idx"
	@makeindex $(NAME).idx >/dev/null 2> /dev/null 2> /dev/null
	@echo "pdflatex $(NAME).tex"
	@pdflatex $(NAME).tex >/dev/null 2> /dev/null
	@echo "pdflatex $(NAME).tex"
	@pdflatex $(NAME).tex >/dev/null 2> /dev/null
	@echo "make clean"
	@make clean > /dev/null 2> /dev/null

clean:
	rm -rf *.aux *.bbl *.blg *.glg *.glo *.gls *.idx  *.ilg *.ind *.ist *.log *.out *.toc *.backup *.xml *.bcf *.lot *.lof