# Created by: Joe Marcus Clarke <marcus@FreeBSD.org>
# $FreeBSD: head/x11/mate/Makefile 412351 2016-04-01 14:33:55Z mat $

PORTNAME=	mate
PORTVERSION=	1.14.0
CATEGORIES=	x11 mate

MAINTAINER=	gnome@FreeBSD.org
COMMENT=	"meta-port" for the MATE integrated X11 desktop

USES=		metaport

RUN_DEPENDS=	mate-base>=1.8.0:x11/mate-base \
		mate-themes>=1.8.0:x11-themes/mate-themes \
		mate-icon-theme-faenza>=1.8.0:x11-themes/mate-icon-theme-faenza \
		mate-terminal:x11/mate-terminal \
		mate-screensaver:x11/mate-screensaver \
		galculator:math/galculator \
		mate-screenshot:deskutils/mate-utils \
		mate-system-monitor:sysutils/mate-system-monitor \
		eom:graphics/eom \
		engrampa:archivers/engrampa \
		atril:graphics/atril \
		mate-volume-control:audio/mate-media \
		mate-power-manager:sysutils/mate-power-manager \
		caja-sendto:deskutils/caja-extensions \
		mozo:deskutils/mozo \
		mate-applets>=1.8.0:x11/mate-applets

USE_MATE=	pluma:run

.include <bsd.port.mk>
