
# Initialize AC: ACINIT( package_name, version, bug_report_address)
AC_INIT([bisquick], [0.1])
# Initialize Automake
AM_INIT_AUTOMAKE([-Wall subdir-objects  foreign])

: ${CXXFLAGS=""}
CFLAGS="$CFLAGS -I/opt/local/include"
CXXFLAGS="$CXXFLAGS -I/opt/local/include"
LDFLAGS="$LDFLAGS -L/opt/local/lib"
AC_PROG_CXX

AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([
	Makefile src/Makefile
])

AC_ARG_WITH([seqan-include-path],
  [AS_HELP_STRING([--seqan-include-path],
    [location of the SeqAn headers, default to seqan-cxx/])],
  [SEQAN_CFLAGS="-I$withval"],
  [SEQAN_CFLAGS='-I../ext/seqan/include/'])
AC_SUBST(SEQAN_CFLAGS)

AC_OUTPUT


dnl # AM stands for Automake commands, AC stands for Autoconf commands
dnl # We use libraries
dnl AC_PROG_RANLIB
dnl # Let's check for a C++ compiler
dnl AC_LANG(C++)
dnl # Let's set a C++ compiler
dnl AC_PROG_CXX
dnl # This suppresses the error we get for also having the cc version of helper library.
dnl AC_SUBST([CC])
dnl # Let's specify where the Makefiles should be produced.
dnl # These are the same locations as your Makefile.in's, but named as Makefile only
dnl # We need to do this because both Autoconf and Automake read this file and
dnl # produce Makefiles from this list.
dnl AC_CONFIG_FILES([Makefile src/Makefile])
dnl # Finally produce "configure" script



dnl : ${CXXFLAGS=""}
dnl CFLAGS="$CFLAGS -I/opt/local/include"
dnl CXXFLAGS="$CXXFLAGS -I/opt/local/include"
dnl LDFLAGS="$LDFLAGS -L/opt/local/lib"
dnl AC_PROG_CXX

dnl AC_ARG_WITH([seqan-include-path],
dnl   [AS_HELP_STRING([--seqan-include-path],
dnl     [location of the SeqAn headers, default to seqan-cxx/])],
dnl   [SEQAN_CFLAGS="-I$withval"],
dnl   [SEQAN_CFLAGS='-Iext/seqan/'])
dnl AC_SUBST(SEQAN_CFLAGS)


dnl AC_OUTPUT
