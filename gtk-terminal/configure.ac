dnl Process this file with autoconf to produce a configure script.

AC_INIT(src/main.c)
AM_CONFIG_HEADER(config.h)

PACKAGE=gtk-terminal
VERSION=0.1

AM_INIT_AUTOMAKE($PACKAGE,$VERSION)

AC_PROG_CC
AC_STDC_HEADERS
AC_PROG_INSTALL

PKG_CHECK_MODULES(DEPS, gtk+-2.0 >= 2.4 glib-2.0 >= 2.4 vte >= 0.11)
AC_SUBST(DEPS_CFLAGS)
AC_SUBST(DEPS_LIBS)

ALL_LINGUAS="zh_CN"
AM_GLIB_GNU_GETTEXT

GETTEXT_PACKAGE=$PACKAGE
AC_SUBST(GETTEXT_PACKAGE)
AC_DEFINE_UNQUOTED([GETTEXT_PACKAGE],["${GETTEXT_PACKAGE}"],[gettext domain])

ALL_LINGUAS="zh_CN"

AC_OUTPUT([
Makefile 
src/Makefile 
pixmaps/Makefile 
po/Makefile.in
])
