.PHONY: pdf, clean, edit

TEXDIR ?= latexfiles
TEXSRC ?= mnras-paper
EDITOR ?= hx

pdf:
	latexmk -pdf -cd $(TEXDIR)/$(TEXSRC).tex
	mv $(TEXDIR)/$(TEXSRC).pdf $(TEXSRC).pdf

clean:
	latexmk -C -cd $(TEXDIR)/$(TEXSRC).tex
	rm $(TEXSRC).pdf

edit:
	$(EDITOR) $(TEXDIR)/$(TEXSRC).tex
