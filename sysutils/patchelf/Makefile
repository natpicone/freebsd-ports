# Created by: William Grzybowski <wg@FreeBSD.org>
# $FreeBSD$

PORTNAME=	patchelf
PORTVERSION=	0.10
PORTREVISION=	1
CATEGORIES=	sysutils

MAINTAINER=	wg@FreeBSD.org
COMMENT=	Utility to modify the dynamic linker

LICENSE=	GPLv3+
LICENSE_FILE=	${WRKSRC}/COPYING

USES=		autoreconf compiler:c++11-lang gmake
USE_GITHUB=	yes
GH_ACCOUNT=	NixOS

GNU_CONFIGURE=	yes

OPTIONS_DEFINE=	DOCS

.include <bsd.port.mk>
