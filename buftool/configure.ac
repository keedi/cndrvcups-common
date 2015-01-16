#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.
AC_INIT([buftool.c], [1.0.0], [krichter722@aol.de])
AC_CONFIG_MACRO_DIR([m4])
LT_INIT
AM_INIT_AUTOMAKE([foreign])
AM_CONFIG_HEADER(config.h)

AC_ARG_ENABLE(progpath)
if test "${enable_progpath}" = "" ; then
   enable_progpath="$prefix/bin"
fi

AC_DEFINE_UNQUOTED(PROG_PATH, "$enable_progpath")
AC_SUBST(PROG_PATH)

# Checks for programs.
AC_PROG_CC
AC_PROG_INSTALL
# AM_PROG_LIBTOOL
AC_PROG_RANLIB

# Checks for libraries.

# Checks for header files.
AC_HEADER_STDC
AC_CHECK_HEADERS([stdlib.h string.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.
AC_FUNC_MALLOC

#AC_CONFIG_FILES([Makefile])
AC_OUTPUT([Makefile])
