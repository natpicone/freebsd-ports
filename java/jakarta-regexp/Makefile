# Created by: Dave Glowacki <dglo@ssec.wisc.edu> #
# $FreeBSD$

PORTNAME=	jakarta-regexp
PORTVERSION=	1.5
PORTREVISION=	3
CATEGORIES=	java devel
MASTER_SITES=	APACHE_JAKARTA/regexp/binaries

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Regular expressions for Java

LICENSE=	APACHE20

DEPRECATED=		EOL: As of 2011-04-17, the Regexp project is retired
EXPIRATION_DATE=	2020-02-29
BROKEN_armv6=		fails to build: build.xml: Java returned: 1
BROKEN_armv7=		fails to build: build.xml: Java returned: 1

USE_JAVA=	yes
USE_ANT=	yes
ALL_TARGET=	test package
MAKE_ARGS=	-Djakarta-site.dir=${WRKSRC}

JAVALIBNAME=	${PORTNAME}-${PORTVERSION}

PLIST_FILES=	${JAVAJARDIR}/${PORTNAME}.jar
PORTDOCS=	*

OPTIONS_DEFINE=	DOCS

do-install:
	@${MKDIR} ${STAGEDIR}${JAVAJARDIR}
	${INSTALL_DATA} ${WRKSRC}/${PORTNAME}-${PORTVERSION}.jar \
		${STAGEDIR}${JAVAJARDIR}/${PORTNAME}.jar
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	(cd ${WRKSRC}/docs/api && ${COPYTREE_SHARE} . ${STAGEDIR}${DOCSDIR})

.include <bsd.port.mk>
