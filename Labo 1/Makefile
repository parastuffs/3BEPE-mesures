all: labo correction
	echo "done"
	

labo: *.tex
	pdflatex -shell-escape -jobname="labo_mesure" labo_mesure.tex
	pdflatex -shell-escape -jobname="labo_mesure" labo_mesure.tex
	

correction: *.tex
	pdflatex -shell-escape -jobname=labo_mesure_correction "\def\koriG{} \input{labo_mesure.tex}"
	pdflatex -shell-escape -jobname=labo_mesure_correction "\def\koriG{} \input{labo_mesure.tex}"
	
clean:
	rm -f labo_mesure_correction.pdf rm labo_mesure.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc *.fls *.fdb_latexmk
	
