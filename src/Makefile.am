libdri2_la_LTLIBRARIES = libdri2.la
libdri2_ladir = $(libdir)
libdri2_la_LDFLAGS = ${XLIBS_CFLAGS}
libdri2_la_LIBADD = -lX11 -lXext
libdri2_la_CFLAGS = ${XLIBS_CFLAGS}

AM_CFLAGS = -I$(top_srcdir)/src 

libdri2_la_SOURCES = dri2.c
libdri2_la_HEADERS = dri2.h

libdri2includedir = ${includedir}/dri2
libdri2include_HEADERS = $(top_srcdir)/src/dri2.h 

