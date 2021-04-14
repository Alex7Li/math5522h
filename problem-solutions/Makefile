all: sol1.pdf sol2.pdf sol3.pdf sol4.pdf sol5.pdf sol6.pdf sol7.pdf sol8.pdf sol9.pdf sol10.pdf sol11.pdf sol12.pdf sol13.pdf sol14.pdf

%.pdf: %.tex
	pdflatex $<
	rm -f sols.aux
	cat *.aux > sols.aux
	cat sols.aux > $(patsubst %.tex,%.aux,$<)
	pdflatex $<
	rm -f sols.aux
