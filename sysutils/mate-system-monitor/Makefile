# Created by: Joe Marcus Clarke <marcus@FreeBSD.org>
# $FreeBSD: head/sysutils/mate-system-monitor/Makefile 412349 2016-04-01 14:25:16Z mat $

PORTNAME=	mate-system-monitor
PORTVERSION=	1.14.1
CATEGORIES=	sysutils mate
MASTER_SITES=	MATE
DIST_SUBDIR=	mate

MAINTAINER=	gnome@FreeBSD.org
COMMENT=	MATE system monitor program

BUILD_DEPENDS=	itstool:textproc/itstool
LIB_DEPENDS=	libgtop-2.0.so:devel/libgtop \
		libdbus-glib-1.so:devel/dbus-glib

PORTSCOUT=	limitw:1,even

USES=		alias compiler:c++11-lang gettext gmake pathfix \
		pkgconfig tar:xz
USE_MATE=	icontheme
USE_GNOME=	gtk30 gtkmm30 intlhack librsvg2 libwnck3 libxml2
GNU_CONFIGURE=	yes
CONFIGURE_ENV=	LIBS="-lutil" DATADIRNAME="share"
CPPFLAGS+=	-I${LOCALBASE}/include
LDFLAGS+=	-L${LOCALBASE}/lib

GLIB_SCHEMAS=	org.mate.system-monitor.enums.xml \
		org.mate.system-monitor.gschema.xml

.include <bsd.port.mk>
