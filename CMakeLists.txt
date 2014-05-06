cmake_minimum_required(VERSION 2.8)

project(NMdE NONE)
include(UseLATEX)

set(CHAPTERS
	title.tex
	chapters/chapter-01.tex
)

set(FIGURES
	figures/chapter-01/mathematik_teilgebiete.tex
	figures/chapter-01/zusammenspiel_mathematik_informatik.tex
)

set(IMAGES
	pics/bisection.png
)

set(LATEX_INPUTS
	${CHAPTERS}
	${FIGURES}
)

add_latex_document(skript.tex DEFAULT_PDF
	INPUTS ${LATEX_INPUTS}
	IMAGES ${IMAGES})