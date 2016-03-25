# Makefile for this project.
# Pablo Cobelli

FILE=ms

all: $(FILE).pdf

.PHONY: clean

edit:
	vim $(FILE).tex

clean:
	@rm *.aux *.blg *.out *.bbl *.log $(FILE).pdf

$(FILE).pdf: $(FILE).tex
	@latexmk  $(FILE)

view:
	@open $(FILE).pdf
