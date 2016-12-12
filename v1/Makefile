TEX = xelatex
RM = rm -f

.PHONY: all view

all : resume.pdf

view :
	open resume.pdf

resume.pdf :
	$(TEX) resume.tex

clean :
	$(RM) resume.pdf resume.aux resume.log resume.out
