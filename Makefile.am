EXTRA_DIST = \
	Paper-Undead

themedir = $(datadir)/icons

install-data-hook:
	$(MKDIR_P) $(DESTDIR)/usr/share/icons
	cp -Rv Paper-Undead $(DESTDIR)/usr/share/icons/.

uninstall-hook:
	test -e $(DESTDIR)/usr/share/icons/Paper-Undead && rm -rfv $(DESTDIR)/usr/share/icons/Paper-Undead
