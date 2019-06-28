include $(top_srcdir)/config/include-Makefile.am

bin_PROGRAMS = getopt

getopt_CPPFLAGS = -DLIBCGETOPT=1 $(AM_CPPFLAGS)
getopt_SOURCES = getopt.c getopt-res.rc

dist_man_MANS = getopt.1

exampledir = $(datadir)/getopt/
dist_example_SCRIPTS = getopt-parse.bash getopt-parse.tcsh \
	getopt-test.bash getopt-test.tcsh

EXTRA_DIST = README Changelog COPYING

