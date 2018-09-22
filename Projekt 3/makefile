PROJEKT=proj3

$(PROJEKT).pdf: $(PROJEKT).ps
	ps2pdf -sPAPERSIZE=a4 $^

$(PROJEKT).ps: $(PROJEKT).dvi
	dvips $^

$(PROJEKT).dvi: $(PROJEKT).tex
	latex $^
	latex $^

pdflatex: $(PROJEKT).tex
	pdflatex $^

clean:
	rm -rf $(PROJEKT)*
