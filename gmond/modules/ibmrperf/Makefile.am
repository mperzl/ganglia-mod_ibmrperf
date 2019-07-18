AM_CFLAGS  = -I$(top_builddir)/include -I$(top_builddir)/lib -I$(top_builddir)/libmetrics

if STATIC_BUILD
noinst_LTLIBRARIES    = libmodibmrperf.la
libmodibmrperf_la_SOURCES = mod_ibmrperf.c 
else
pkglib_LTLIBRARIES    = modibmrperf.la
modibmrperf_la_SOURCES = mod_ibmrperf.c 
modibmrperf_la_LDFLAGS = -module -avoid-version
modibmrperf_la_LIBADD = $(top_builddir)/libmetrics/libmetrics.la

EXTRA_DIST = ../conf.d/ibmrperf.conf
endif

INCLUDES = @APR_INCLUDES@

