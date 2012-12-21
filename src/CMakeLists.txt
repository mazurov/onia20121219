# Note that normally CMakeLists.txt would not be considered an
# input to the document, but in this special case of documenting
# UseLATEX.cmake the contents of this file is actually included
# in the document.
FILE(GLOB INCLUDES RELATIVE ${CMAKE_CURRENT_SOURCE_DIR} "*.inc.tex")
SET(IMAGES
    images/m3p.png
    images/plot_stat_mean_2p.png
    images/plot_stat_mean_3p.png
    images/plot_rerr_m3p.png
    images/splot.png
    images/fit.png
    images/spectr.png
    images/mumu.png
    images/ups.png
    images/mcdkfiles.png
    images/chibY2S.png
    images/chibY3S.png
    )
ADD_LATEX_DOCUMENT(onia20121218.tex INPUTS ${INCLUDES} IMAGES ${IMAGES} DEFAULT_PDF)
