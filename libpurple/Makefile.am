EXTRA_DIST = \
		dbus-analyze-functions.py \
		dbus-analyze-signals.py \
		dbus-analyze-types.py \
		enums.c.in \
		enums.h.in \
		glibcompat.h \
		marshallers.list \
		purple-notifications-example \
		purple-remote \
		purple-send \
		purple-send-async \
		purple-url-handler \
		purple.h.in \
		tag.sh \
		version.h.in \
		Makefile.mingw \
		data/purple-3.pc.in \
		data/purple-3-uninstalled.pc.in \
		win32/global.mak \
		win32/libc_interface.c \
		win32/libc_interface.h \
		win32/libc_internal.h \
		win32/libpurplerc.rc.in \
		win32/rules.mak \
		win32/targets.mak \
		win32/wpurpleerror.h \
		win32/win32dep.c \
		win32/giowin32.c \
		win32/win32dep.h

if USE_GCONFTOOL
GCONF_DIR=data/gconf
endif

SUBDIRS = $(GCONF_DIR) . plugins protocols tests example

purple_coresources = \
	account.c \
	accounts.c \
	accountopt.c \
	blistnode.c \
	blistnodetypes.c \
	buddylist.c \
	buddyicon.c \
	certificate.c \
	ciphers/aescipher.c \
	ciphers/descipher.c \
	ciphers/des3cipher.c \
	ciphers/hmaccipher.c \
	ciphers/md4hash.c \
	ciphers/md5hash.c \
	ciphers/pbkdf2cipher.c \
	ciphers/rc4cipher.c \
	ciphers/sha1hash.c \
	ciphers/sha256hash.c \
	cipher.c \
	circularbuffer.c \
	cmds.c \
	connection.c \
	conversation.c \
	conversationtypes.c \
	conversations.c \
	core.c \
	debug.c \
	desktopitem.c \
	e2ee.c \
	eventloop.c \
	http.c \
	idle.c \
	image.c \
	image-store.c \
	keyring.c \
	log.c \
	media/backend-fs2.c \
	media/backend-iface.c \
	media/candidate.c \
	media/codec.c \
	media/enum-types.c \
	media.c \
	mediamanager.c \
	memorypool.c \
	message.c \
	mime.c \
	nat-pmp.c \
	network.c \
	ntlm.c \
	notify.c \
	plugin.c \
	pluginpref.c \
	pounce.c \
	prefs.c \
	presence.c \
	proxy.c \
	prpl.c \
	purple-socket.c \
	request.c \
	request-datasheet.c \
	roomlist.c \
	savedstatuses.c \
	server.c \
	signals.c \
	smiley-custom.c \
	smiley-list.c \
	smiley-parser.c \
	smiley-theme.c \
	smiley.c \
	dnsquery.c \
	dnssrv.c\
	status.c \
	stringref.c \
	stun.c \
	sound.c \
	sound-theme.c \
	sound-theme-loader.c \
	sslconn.c \
	theme.c \
	theme-loader.c \
	theme-manager.c \
	trie.c \
	upnp.c \
	util.c \
	version.c \
	whiteboard.c \
	xfer.c \
	xmlnode.c

purple_builtsources = \
	enums.c \
	marshallers.c

purple_coreheaders = \
	account.h \
	accounts.h \
	accountopt.h \
	blistnode.h \
	blistnodetypes.h \
	buddylist.h \
	buddyicon.h \
	certificate.h \
	cipher.h \
	circularbuffer.h \
	cmds.h \
	connection.h \
	conversation.h \
	conversationtypes.h \
	conversations.h \
	core.h \
	dbus-maybe.h \
	debug.h \
	desktopitem.h \
	e2ee.h \
	eventloop.h \
	http.h \
	idle.h \
	image.h \
	image-store.h \
	keyring.h \
	log.h \
	media.h \
	media-gst.h \
	mediamanager.h \
	memorypool.h \
	message.h \
	mime.h \
	nat-pmp.h \
	network.h \
	notify.h \
	ntlm.h \
	plugin.h \
	pluginpref.h \
	pounce.h \
	prefs.h \
	presence.h \
	proxy.h \
	prpl.h \
	purple-socket.h \
	request.h \
	request-datasheet.h \
	roomlist.h \
	savedstatuses.h \
	server.h \
	signals.h \
	smiley-custom.h \
	smiley-list.h \
	smiley-parser.h \
	smiley-theme.h \
	smiley.h \
	dnsquery.h \
	dnssrv.h \
	status.h \
	stringref.h \
	stun.h \
	sound.h \
	sound-theme.h \
	sound-theme-loader.h \
	sslconn.h \
	theme.h \
	theme-loader.h \
	theme-manager.h \
	trie.h \
	upnp.h \
	util.h \
	whiteboard.h \
	xfer.h \
	xmlnode.h

if IS_WIN32
purple_coresources += \
	win32/giowin32.c \
	win32/libc_interface.c \
	win32/win32dep.c

purple_coreheaders += \
	win32/libc_interface.h \
	win32/libc_internal.h \
	win32/win32dep.h \
	win32/wpurpleerror.h

.rc.o: %.rc
	$(AM_V_GEN)$(WINDRES) -i $< -o $@

LIBPURPLE_WIN32RES = win32/libpurplerc.o
LIBPURPLE_WIN32RES_LDFLAGS = -Wl,$(LIBPURPLE_WIN32RES)
endif

purple_mediaheaders = \
	backend-iface.h \
	candidate.h \
	codec.h \
	enum-types.h

purple_cipherheaders = \
	aescipher.h \
	descipher.h \
	des3cipher.h \
	hmaccipher.h \
	md4hash.h \
	md5hash.h \
	pbkdf2cipher.h \
	rc4cipher.h \
	sha1hash.h \
	sha256hash.h

purple_builtheaders = purple.h version.h enums.h marshallers.h

purple_enumheaders = \
	$(srcdir)/account.h \
	$(srcdir)/cipher.h \
	$(srcdir)/connection.h \
	$(srcdir)/conversation.h \
	$(srcdir)/conversationtypes.h \
	$(srcdir)/roomlist.h \
	$(srcdir)/status.h \
	$(srcdir)/xfer.h

marshallers.h: marshallers.list
	$(AM_V_GEN)$(GLIB_GENMARSHAL) --prefix=purple_smarshal $(srcdir)/marshallers.list --header > marshallers.h

marshallers.c: marshallers.list marshallers.h
	$(AM_V_GEN)echo "#include \"marshallers.h\"" > marshallers.c
	$(AM_V_at)$(GLIB_GENMARSHAL) --prefix=purple_smarshal $(srcdir)/marshallers.list --body >> marshallers.c

enums.h: $(srcdir)/enums.h.in $(purple_enumheaders)
	$(AM_V_GEN)$(GLIB_MKENUMS) --template $(srcdir)/enums.h.in $(purple_enumheaders) > $@

enums.c: $(srcdir)/enums.c.in $(purple_enumheaders)
	$(AM_V_GEN)$(GLIB_MKENUMS) --template $(srcdir)/enums.c.in $(purple_enumheaders) > $@

CLEANFILES = \
	enums.c \
	enums.h \
	marshallers.c \
	marshallers.h

if ENABLE_DBUS

CLEANFILES += \
	dbus-bindings.c \
	dbus-client-binding.c \
	dbus-client-binding.h \
	dbus-signals.c \
	dbus-types.c \
	dbus-types.h \
	purple-client-bindings.c \
	purple-client-bindings.h \
	purple.service

# purple dbus server

dbus_sources  = dbus-server.c dbus-useful.c
dbus_headers  = dbus-bindings.h dbus-purple.h dbus-server.h dbus-useful.h dbus-define-api.h dbus-types.h

dbus_exported = dbus-useful.h dbus-define-api.h account.h accounts.h blistnode.h \
                blistnodetypes.h buddylist.h buddyicon.h connection.h conversation.h \
                conversationtypes.h conversations.h core.h xfer.h log.h notify.h \
                prefs.h presence.h roomlist.h savedstatuses.h smiley.h smiley-list.h \
                status.h server.h util.h xmlnode.h prpl.h

purple_build_coreheaders = $(addprefix $(srcdir)/, $(purple_coreheaders)) \
		$(addprefix $(srcdir)/ciphers/, $(purple_cipherheaders)) \
		$(addprefix $(srcdir)/media/, $(purple_mediaheaders)) \
		$(purple_builtheaders)
dbus_build_exported = $(addprefix $(srcdir)/, $(dbus_exported))
# We should probably make this better
dbus_signals = $(addprefix $(srcdir)/, $(purple_coresources)) \
	$(srcdir)/protocols/irc/irc.c \
	$(srcdir)/protocols/jabber/libxmpp.c

dbus-types.c: dbus-analyze-types.py $(purple_build_coreheaders)
	$(AM_V_GEN)cat $(purple_build_coreheaders) | $(PYTHON) $(srcdir)/dbus-analyze-types.py --pattern=PURPLE_DBUS_DEFINE_TYPE\(%s\) > $@

dbus-types.h: dbus-analyze-types.py $(purple_build_coreheaders)
	$(AM_V_GEN)cat $(purple_build_coreheaders) | $(PYTHON) $(srcdir)/dbus-analyze-types.py --pattern=PURPLE_DBUS_DECLARE_TYPE\(%s\) > $@

dbus-bindings.c: dbus-analyze-functions.py $(dbus_exported)
	$(AM_V_GEN)cat $(dbus_build_exported) | $(PYTHON) $(srcdir)/dbus-analyze-functions.py > $@

dbus-signals.c: dbus-analyze-signals.py $(dbus_signals)
	$(AM_V_GEN)cat $(dbus_signals) | $(PYTHON) $(srcdir)/dbus-analyze-signals.py > $@

dbus-server.$(OBJEXT): dbus-bindings.c dbus-signals.c dbus-types.c dbus-types.h
dbus-server.lo: dbus-bindings.c dbus-signals.c dbus-types.c dbus-types.h
$(libpurple_la_OBJECTS): dbus-types.h

# libpurple-client

libpurple_client_lib = libpurple-client.la

libpurple_client_la_SOURCES = purple-client.c purple-client.h
libpurple_client_la_LDFLAGS = -version-info $(PURPLE_LT_VERSION_INFO) -no-undefined
libpurple_client_la_LIBADD = $(DBUS_LIBS)

purple-client-bindings.c: dbus-analyze-functions.py $(dbus_exported)
	$(AM_V_GEN)cat $(dbus_build_exported) | $(PYTHON) $(srcdir)/dbus-analyze-functions.py --client > $@

purple-client-bindings.h: dbus-analyze-types.py dbus-analyze-functions.py $(purple_coreheaders) $(addprefix ciphers/, $(purple_cipherheaders)) $(addprefix media/, $(purple_mediaheaders)) $(purple_builtheaders) $(dbus_exported)
	$(AM_V_GEN)cat $(purple_build_coreheaders) | $(PYTHON) $(srcdir)/dbus-analyze-types.py --keyword=enum --verbatim > $@
	$(AM_V_at)cat $(dbus_build_exported) | $(PYTHON) $(srcdir)/dbus-analyze-functions.py --client --headers >> $@

$(libpurple_client_la_OBJECTS): purple-client-bindings.h purple-client-bindings.c

# purple-client-example

purple_client_example_SOURCES = purple-client-example.c

purple_client_example_DEPENDENCIES = libpurple-client.la

purple_client_example_LDADD = \
	libpurple-client.la \
	$(GLIB_LIBS) \
	$(DBUS_LIBS)

bin_PROGRAMS = purple-client-example

purple-client-example.$(OBJEXT): purple-client-bindings.h

# scripts

bin_SCRIPTS = purple-remote purple-send purple-send-async purple-url-handler

BUILT_SOURCES = $(purple_builtheaders) \
	$(purple_builtsources) \
	dbus-bindings.c \
	dbus-signals.c \
	dbus-types.c \
	dbus-types.h \
	purple-client-bindings.c \
	purple-client-bindings.h

else

BUILT_SOURCES = $(purple_builtheaders) $(purple_builtsources)

endif

lib_LTLIBRARIES = libpurple.la $(libpurple_client_lib)

libpurple_la_SOURCES = \
	$(purple_coresources) \
	$(purple_builtsources) \
	$(dbus_sources)

noinst_HEADERS= \
	internal.h \
	media/backend-fs2.h \
	valgrind.h

libpurpleincludedir=$(includedir)/libpurple
libpurpleinclude_HEADERS = \
	$(purple_coreheaders) \
	$(purple_builtheaders) \
	$(dbus_headers)

cipherincludedir=$(includedir)/libpurple/ciphers
cipherinclude_HEADERS = \
	$(addprefix $(srcdir)/ciphers/, $(purple_cipherheaders))

mediaincludedir=$(includedir)/libpurple/media
mediainclude_HEADERS = \
	$(addprefix $(srcdir)/media/, $(purple_mediaheaders))

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = data/purple-3.pc

libpurple_la_DEPENDENCIES = \
	$(STATIC_LINK_LIBS) $(LIBPURPLE_WIN32RES)

libpurple_la_LDFLAGS = -export-dynamic -version-info $(PURPLE_LT_VERSION_INFO) \
	-no-undefined $(LIBPURPLE_WIN32RES_LDFLAGS)
libpurple_la_LIBADD = \
	$(STATIC_LINK_LIBS) \
	$(DBUS_LIBS) \
	$(DNSAPI_LIBS) \
	$(GLIB_LIBS) \
	$(LIBXML_LIBS) \
	$(NETWORKMANAGER_LIBS) \
	$(INTLLIBS) \
	$(FARSTREAM_LIBS) \
	$(GSTREAMER_LIBS) \
	$(GSTVIDEO_LIBS) \
	$(GSTAPP_LIBS) \
	$(GSTINTERFACES_LIBS) \
	$(IDN_LIBS) \
	$(JSON_LIBS) \
	$(GNUTLS_LIBS) \
	$(NSS_LIBS) \
	$(ZLIB_LIBS) \
	-lm

AM_CPPFLAGS = \
	$(GLIB_CFLAGS) \
	$(DEBUG_CFLAGS) \
	$(DBUS_CFLAGS) \
	$(LIBXML_CFLAGS) \
	$(FARSTREAM_CFLAGS) \
	$(GSTREAMER_CFLAGS) \
	$(GSTVIDEO_CFLAGS) \
	$(GSTAPP_CFLAGS) \
	$(GSTINTERFACES_CFLAGS) \
	$(IDN_CFLAGS) \
	$(NETWORKMANAGER_CFLAGS) \
	$(JSON_CFLAGS) \
	$(GNUTLS_CFLAGS) \
	$(NSS_CFLAGS) \
	$(ZLIB_CFLAGS)
