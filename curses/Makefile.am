## Process this file with automake to produce Makefile.in

AUTOMAKE_OPTIONS = 1.4 foreign

# A list of all the files in the current directory which can be regenerated
MAINTAINERCLEANFILES = Makefile.in

SUBDIRS = curses test

CFLAGS_EXTRA = -I$(includedir) -I$(top_srcdir)

EXTRA_DIST = INSTALL

install-data-local:
	@$(NORMAL_INSTALL)
	if test -z "$DESTDIR"; then \
		$(prefix)/bin/feritedoc --regenerate ; \
	fi
