#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ(2.61)
AC_INIT(util-linux-ng, 2.14.1, kzak@redhat.com)
AC_CONFIG_SRCDIR([getopt/getopt.c])
AC_CONFIG_HEADER([config.h])
AM_INIT_AUTOMAKE

# Checks for programs.
AC_PROG_CC
AC_PROG_MAKE_SET
AC_GNU_SOURCE
AM_PROG_CC_C_O
AC_PROG_RANLIB

# Checks for libraries.
# FIXME: Replace `main' with a function in `-ltermcap':
#AC_CHECK_LIB([termcap], [main])

# Checks for header files.
AC_HEADER_DIRENT
AC_HEADER_STDC
AC_CHECK_HEADERS([fcntl.h langinfo.h libintl.h locale.h malloc.h paths.h stdint.h stdlib.h string.h strings.h sys/file.h sys/ioctl.h sys/param.h sys/time.h unistd.h wchar.h wctype.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_C_CONST
AC_C_INLINE
AC_TYPE_INT64_T
AC_TYPE_MODE_T
AC_TYPE_OFF_T
AC_TYPE_PID_T
AC_TYPE_SIZE_T
AC_TYPE_SSIZE_T
AC_HEADER_TIME
AC_STRUCT_TM
AC_TYPE_UID_T
AC_TYPE_UINT16_T
AC_TYPE_UINT32_T
AC_TYPE_UINT64_T
AC_TYPE_UINT8_T
AC_CHECK_TYPES([u_int, u_char, quad_t, u_quad_t])

# Checks for library functions.
AC_FUNC_ALLOCA
AC_FUNC_CLOSEDIR_VOID
AC_FUNC_LSTAT
AC_FUNC_LSTAT_FOLLOWS_SLASHED_SYMLINK
AC_FUNC_MALLOC
AC_FUNC_MEMCMP
AC_FUNC_REALLOC
AC_FUNC_STAT
AC_FUNC_VPRINTF
AC_CHECK_FUNCS([bcopy bzero getcwd gettimeofday index iswprint memmove memset nl_langinfo random setlocale srandom strcasecmp strchr strerror strncasecmp strrchr strspn strstr strtol wcwidth])

AM_GNU_GETTEXT_VERSION([0.14.1])
AM_GNU_GETTEXT([external])
if test -d "$srcdir/po"
then
    ALL_LINGUAS=`cd $srcdir/po > /dev/null && echo *.po | sed 's/\.po//g'`
else
    ALL_LINGUAS="af am ar as be bg bn_IN bn ca cs cy da de el en_GB es et eu_ES fa fi fr gl gu he hi hr hu hy id is it ja ka kn ko ku lo lt lv mk ml mr ms my nb nl nn no nso or pa pl pt_BR pt ro ru si sk sl sq sr@Latn sr sv ta te th tr uk ur vi zh_CN zh_TW zu"
fi


AC_CONFIG_FILES([Makefile
                 lib/Makefile
                 getopt/Makefile
                 include/Makefile
                 misc-utils/Makefile
			  po/Makefile.in
                 text-utils/Makefile])
AC_OUTPUT
