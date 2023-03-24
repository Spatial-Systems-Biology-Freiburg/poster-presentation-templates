.PHONY: main clean FORCE

main: poster.pdf

poster.pdf: FORCE
	latexmk -pdflatex='lualatex -interaction nonstopmode' --output-directory=out -pdf poster.tex

clean:
	rm -f out/*.aux
	rm -f out/*.pdf
	rm -f out/*.bib
	rm -f out/*.bbl
	rm -f out/*.fdb_latexmk
	rm -f out/*.fls
	rm -f out/*.log


fresh: clean main
