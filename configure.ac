AC_INIT([addusergtk], [0.0.1], [])
AC_CONFIG_SRCDIR([Makefile.am])
AC_CONFIG_HEADERS(config.h)
AM_INIT_AUTOMAKE([])
AM_MAINTAINER_MODE

AC_PROG_CC
AM_PROG_CC_C_O

AM_PROG_VALAC([0.30.0])

AC_SUBST(CFLAGS)
AC_SUBST(CPPFLAGS)
AC_SUBST(LDFLAGS)

GLIB_REQUIRED=2.12.0
GTK_REQUIRED=3.0.8

PKG_CHECK_MODULES(addusergtk, glib-2.0 >= $GLIB_REQUIRED gtk+-3.0 >= $GTK_REQUIRED)

AC_SUBST(addusergtk_CFLAGS)
AC_SUBST(addusergtk_LIBS)
AC_PROG_LN_S

VALA_PACKAGES="--pkg posix --pkg gtk+-3.0"

AC_SUBST(VALA_PACKAGES)

AC_PREFIX_DEFAULT("/usr")

AC_CONFIG_FILES([Makefile
        gui/Makefile
        shell/Makefile
        ])



AC_OUTPUT
