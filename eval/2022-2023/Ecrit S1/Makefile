all: labo correction
#	labo
#	correction
	echo "done"


labo: *.tex
	#cd Figures; ./crop.sh;cd ..
	#cp ~/Documents/SIES2013add.bib .
	pdflatex -shell-escape -jobname="Mesures_exam_1s2022-23" Mesures_exam_1s2022-23.tex
	#bibtex SIES_2013_YAllard.aux
	#pdflatex labo_diodes_corr.tex
	pdflatex -shell-escape -jobname="Mesures_exam_1s2022-23" Mesures_exam_1s2022-23.tex


correction: *.tex
	#cd Figures; ./crop.sh;cd ..
	#cp ~/Documents/SIES2013add.bib .
	pdflatex -shell-escape -jobname=Mesures_exam_1s2022-23_correction "\def\koriG{} \input{Mesures_exam_1s2022-23.tex}"
	#bibtex SIES_2013_YAllard.aux
	#pdflatex labo_diodes_corr.tex
	pdflatex -shell-escape -jobname=Mesures_exam_1s2022-23_correction "\def\koriG{} \input{Mesures_exam_1s2022-23.tex}"

clean:
	rm -f Mesures_exam_1s2022-23_correction.pdf rm Mesures_exam_1s2022-23.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc
