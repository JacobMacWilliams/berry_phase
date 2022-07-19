.PHONY: main clean

main:
	TEXINPUTS=./texmf//: pdflatex -interaction=batchmode -output-directory=out main.tex
	biber --onlylog out/main.bcf
	# Compile toc/bib
	TEXINPUTS=./texmf//: pdflatex -interaction=batchmode -output-directory=out main.tex
	mv out/main.pdf ./

clean:
	rm -rf out/* main.pdf

