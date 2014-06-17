cmake_minimum_required(VERSION 2.8)

project(NMdE NONE)
include(UseLATEX)

set(CHAPTERS
	title.tex
	chapters/chapter-01.tex
	chapters/chapter-02.tex
	chapters/chapter-03.tex
)

set(FIGURES
	figures/arbeitspunkt.tex
	figures/fixpunktiteration.tex
	figures/intervallhalbierung.tex
	figures/loesung_mathematisches_problem.tex
	figures/mathematik_teilgebiete.tex
	figures/newton_iteration.tex
	figures/schaltung_beispiel_1.tex
	figures/schaltung_beispiel_2.tex
	figures/zusammenspiel_mathematik_informatik.tex
	figures/steepest_descent.tex
	figures/stueckweise_lin_interpolation.tex
	figures/newton_cotes_linear.tex
	figures/newton_cotes_quadratisch.tex
	figures/newton_cotes_multi.tex
	figures/schaltung_transiente_analyse.tex
	figures/schaltung_transiente_analyse_diagramm.tex
)

set(IMAGES)

set(LATEX_INPUTS
	${CHAPTERS}
	${FIGURES}
)

add_latex_document(skript.tex DEFAULT_PDF
	INPUTS ${LATEX_INPUTS}
	IMAGES ${IMAGES})