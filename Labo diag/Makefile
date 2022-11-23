all: labo correction
	echo "done"
	

labo: *.tex
	pdflatex -shell-escape -jobname="labo_mesure_diag" labo_mesure_diag.tex
	pdflatex -shell-escape -jobname="labo_mesure_diag" labo_mesure_diag.tex
	

correction: *.tex
	pdflatex -shell-escape -jobname=labo_mesure_diag_correction "\def\koriG{} \input{labo_mesure_diag.tex}"
	pdflatex -shell-escape -jobname=labo_mesure_diag_correction "\def\koriG{} \input{labo_mesure_diag.tex}"
	
clean:
	rm -f labo_mesure_diag_correction.pdf rm labo_mesure_diag.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc *.fls *.fdb_latexmk
	
