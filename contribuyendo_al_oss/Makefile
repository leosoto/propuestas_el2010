#  LaTeX Makefile
#
#  This file is based on the original work of Jason Blevins 
#  <jrblevin@sdf.lonestar.org>, 2006
#
#  --------------------------------------------------------------
#
#  History
#
#  Version 1: (27/07/2010)
#   - Author: Miguel Angel Ruiz Manzano <mruiz@openminds.cl>
#  Version 1.1: (06/08/2010)
#   - Author: Miguel Angel Ruiz Manzano <mruiz@openminds.cl>
#   - Adopted Attribution-NonCommercial-ShareAlike 3.0 Unported 
#   as license.
#
#  --------------------------------------------------------------
#
#  This file is distributed under the terms and conditions of the
#  Attribution-NonCommercial-ShareAlike 3.0 Unported license. For
#  more information, please visit the following URL
#
#  http://creativecommons.org/licenses/by-nc-sa/3.0/
#
#



###############################################################################
# Configuration Section
# This should be the only section you need to modify

# Project base filename where your main tex file is $(BASENAME).tex
BASENAME = paper

###############################################################################
# File lists

DISTFILES = *.aux *.lo* *~ *.blg *.bbl *.dvi *.toc .*xml *.bak
CLEANFILES = $(DISTFILES) *.ps $(BASENAME)*.pdf *.zip *.tar.gz

###############################################################################
# Build rules

all: clean $(BASENAME).pdf

$(BASENAME).pdf:
	pdflatex $(BASENAME).tex && pdflatex $(BASENAME)_ciego.tex

###############################################################################
# Clean-up rules

clean:
	-rm -f $(CLEANFILES)

distclean:
	-rm -f $(DISTFILES)

