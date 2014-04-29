cmake_minimum_required(VERSION 2.8)

project(NMdE NONE)
include(UseLATEX)

set(CHAPTERS
	title.tex
	chapters/chapter-01.tex
)

set(IMAGES
	pics/bisection.png
)

add_latex_document(skript.tex DEFAULT_PDF
	INPUTS ${CHAPTERS}
	IMAGES ${IMAGES})