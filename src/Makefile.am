bin_PROGRAMS = xarchiver

SUBDIRS = xdgmime

xarchiver_SOURCES = \
	7zip.c \
	7zip.h \
	add_dialog.c \
	add_dialog.h \
	appimage.c \
	appimage.h \
	ar.c \
	ar.h \
	archive.c \
	archive.h \
	arj.c \
	arj.h \
	cpio.c \
	cpio.h \
	date_utils.c \
	date_utils.h \
	exe.c \
	exe.h \
	extract_dialog.c \
	extract_dialog.h \
	gzip_et_al.c \
	gzip_et_al.h \
	interface.c \
	interface.h \
	iso.c \
	iso.h \
	lha.c \
	lha.h \
	main.c \
	main.h \
	mime.c \
	mime.h \
	new_dialog.c \
	new_dialog.h \
	open-with-dlg.c \
	open-with-dlg.h \
	pref_dialog.c \
	pref_dialog.h \
	rar.c \
	rar.h \
	rpm.c \
	rpm.h \
	socket.c \
	socket.h \
	squashfs.c \
	squashfs.h \
	string_utils.c \
	string_utils.h \
	support.h \
	tar.c \
	tar.h \
	unar.c \
	unar.h \
	utf8-fnmatch.c \
	utf8-fnmatch.h \
	window.c \
	window.h \
	zip.c \
	zip.h \
	zpaq.c \
	zpaq.h

if GTK_V2_16
else
xarchiver_SOURCES += sexy-icon-entry.c sexy-icon-entry.h
endif

xarchiver_CFLAGS = \
	-Wall \
	-Wextra \
	-Wno-unused-parameter \
	@GTK_CFLAGS@ \
	-DHTMLDIR=\"$(htmldir)\" \
	-DLOCALEDIR=\"$(localedir)\" \
	-DPIXMAPSDIR=\"$(PIXMAPDIR)\"

xarchiver_CFLAGS += -Wno-deprecated-declarations

xarchiver_LDADD = \
	xdgmime/libxdgmime.la \
	@GTK_LIBS@
