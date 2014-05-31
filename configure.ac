# Process this file with autoconf to produce a configure script.

AC_PREREQ(2.61)
AC_INIT(libdri2, 2.1, [http://])
AC_CONFIG_SRCDIR([src/dri2.c])
AC_CONFIG_HEADER([config.h])

AM_INIT_AUTOMAKE([dist-bzip2])

# Checks for programs.
AC_PROG_LIBTOOL
AC_PROG_CC

# Checks for pkg-configs
PKG_CHECK_MODULES(XLIBS, x11 xext xfixes)
AC_SUBST(XLIBS_CFLAGS)
AC_SUBST(XLIBS_LIBS)

PKG_CHECK_MODULES(DRI2PROTO, dri2proto)
AC_SUBST(DRI2PROTO_CFLAGS)
AC_SUBST(DRI2PROTO_LIBS)

#PKG_CHECK_MODULES(GFXPERF, gfxperf)
#AC_SUBST(GFXPERF_CFLAGS)
#AC_SUBST(GFXPERF_LIBS)


###
pkgconfigdir=${libdir}/pkgconfig/
AC_SUBST(pkgconfigdir)


AC_CONFIG_FILES([Makefile
                 src/Makefile
				 libdri2.pc])
AC_OUTPUT
