ALL=01-intro.pdf 01-applications.pdf 02-syntax.pdf 03-morphology.pdf 05-adding.pdf 05-resources_tools.pdf 05-infrastructure.pdf

all: $(ALL)

01-intro.pdf: 01-intro.tex
	xelatex $<

01-applications.pdf: 01-applications.tex
	xelatex $<

02-syntax.pdf: 02-syntax.tex
	xelatex $<

03-morphology.pdf: 03-morphology.tex
	xelatex $<

05-adding.pdf: 05-adding.tex
	xelatex $<

05-resources_tools.pdf: 05-resources_tools.tex
	xelatex $<

05-infrastructure.pdf: 05-infrastructure.tex
	xelatex $<

unidive-ud-slides.pdf: $(ALL)
	pdfjoin $(ALL) -o $@

clean:
	rm -f $(ALL) *.aux *.log *.out *.vrb *.nav *.snm *.toc
