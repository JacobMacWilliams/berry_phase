.PHONY: main clean

main:
	TEXINPUTS=./texmf//: pdflatex -interaction=batchmode -output-directory=out beamer_title.tex
	# biber --onlylog out/main.bcf
	# Compile toc/bib
	TEXINPUTS=./texmf//: pdflatex -interaction=batchmode -output-directory=out beamer_title.tex
	mv out/beamer_title.pdf ./

clean:
	rm -rf out/* beamer_title.pdf

