cmake_minimum_required(VERSION 2.8)

project(NMdE NONE)
include(UseLATEX)

set(CHAPTERS
	title.tex
	chapters/chapter-01.tex
)

set(FIGURES
	figures/chapter-01/arbeitspunkt.tex
	figures/chapter-01/fixpunktiteration.tex
	figures/chapter-01/intervallhalbierung.tex
	figures/chapter-01/loesung_mathematisches_problem.tex
	figures/chapter-01/mathematik_teilgebiete.tex
	figures/chapter-01/newton_iteration.tex
	figures/chapter-01/schaltung_beispiel_1.tex
	figures/chapter-01/schaltung_beispiel_2.tex
	figures/chapter-01/zusammenspiel_mathematik_informatik.tex
	figures/chapter-01/steepest_descent.tex
	figures/chapter-01/stueckweise_lin_interpolation.tex
	figures/chapter-01/newton_cotes_linear.tex
	figures/chapter-01/newton_cotes_quadratisch.tex
	figures/chapter-01/newton_cotes_multi.tex
)

set(IMAGES)

set(LATEX_INPUTS
	${CHAPTERS}
	${FIGURES}
)

add_latex_document(skript.tex DEFAULT_PDF
	INPUTS ${LATEX_INPUTS}
	IMAGES ${IMAGES})