include $(top_srcdir)/config/include-Makefile.am

EXTRA_DIST = README.clear README.col

bin_PROGRAMS = col colcrt colrm hexdump rev line tailf

LIBS += -L$(top_builddir)/lib -lutil-linux
		  
col_SOURCES = col.c col-res.rc
colcrt_SOURCES = colcrt.c colcrt-res.rc
colrm_SOURCES = colrm.c colrm-res.rc
hexdump_SOURCES = hexdump.c conv.c display.c hexsyntax.c odsyntax.c parse.c \
		  hexdump.h hexdump-res.rc
rev_SOURCES = rev.c rev-res.rc
line_SOURCES = line.c line-res.rc
tailf_SOURCES = tailf.c tailf-res.rc

dist_man_MANS = col.1 colcrt.1 colrm.1 hexdump.1 rev.1 line.1 tailf.1

