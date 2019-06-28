include $(top_srcdir)/config/include-Makefile.am

SUBDIRS = \
	include \
	lib \
	getopt \
	misc-utils \
	po \
	text-utils

ACLOCAL_AMFLAGS = -I m4

EXTRA_DIST = \
		autogen.sh \
		README.devel \
		README.licensing \
		DEPRECATED \
		licenses \
		example.files \
		po/update-potfiles \
		tools \
		docs

distclean-local:
	-find . -name \*~ -o -name \*.orig -o -name \*.rej | xargs rm -f
	rm -rf autom4te.cache
