plugindir = $(libdir)/nautilus-sendto/plugins

INCLUDES =                                      \
        -DDATADIR=\"$(datadir)\"                \
        -DICONDIR=\"$(icondir)\"                \
	-DLOCALEDIR="\"$(datadir)/locale\""	\
        -I$(top_srcdir)/src                     \
        -I$(top_builddir)                       \
        -I$(srcdir)/../				\
        $(NAUTILUS_SENDTO_CFLAGS)               \
        $(DISABLE_DEPRECATED)			\
	$(WARN_CFLAGS)

plugin_LTLIBRARIES = libnstremovable_devices.la

libnstremovable_devices_la_SOURCES = removable-devices.c
libnstremovable_devices_la_LDFLAGS = -module -avoid-version
libnstremovable_devices_la_LIBADD = $(GIO_LIBS) $(NAUTILUS_SENDTO_LIBS) $(builddir)/../libnstcommon.la

