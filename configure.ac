AC_INIT(osm-gps-map, 0.5.0)
AM_INIT_AUTOMAKE(AC_PACKAGE_NAME, AC_PACKAGE_VERSION)

AC_CONFIG_SRCDIR(osmgpsmap.pc.in)
AM_CONFIG_HEADER(config.h)

AM_MAINTAINER_MODE

AC_ISC_POSIX
AC_PROG_CC
AM_PROG_CC_STDC
AC_HEADER_STDC

AM_PROG_LIBTOOL

m4_ifdef([AM_SILENT_RULES],[AM_SILENT_RULES([yes])])

PKG_CHECK_MODULES(OPENSTREETMAP_GPS_MAP, [gtk+-2.0 libsoup-2.4 glib-2.0 >= 2.18 cairo >= 1.8])
AC_SUBST(OPENSTREETMAP_GPS_MAP_CFLAGS)
AC_SUBST(OPENSTREETMAP_GPS_MAP_LIBS)

CFLAGS="$CFLAGS -Wall -Wswitch-enum"

AC_OUTPUT([
osmgpsmap.pc
Makefile
src/Makefile
])

echo
echo $PACKAGE v$VERSION
echo
echo Prefix............... : $prefix
echo
