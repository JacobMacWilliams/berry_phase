.PHONY: main clean

main:
	TEXINPUTS=./texmf//: pdflatex -interaction=batchmode -output-directory=out berry_loop.tex
	mv out/berry_loop.pdf ./
	cp berry_loop.pdf ../

clean:
	rm -rf out/* berry_loop.pdf ../berry_loop.pdf

