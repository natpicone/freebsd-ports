# Created by: Matthias Petermann <matthias@petermann-it.de>
# $FreeBSD$

PORTNAME=	trytond28_analytic_sale
PORTVERSION=	2.8.0
PORTREVISION=	3
CATEGORIES=	finance python
MASTER_SITES=	https://pypi.python.org/packages/source/t/trytond_analytic_sale/ \
		http://downloads-cdn.tryton.org/${PORTVERSION:R}/
DISTNAME=	trytond_analytic_sale-${PORTVERSION}

MAINTAINER=	matthias@petermann-it.de
COMMENT=	Tryton Application Platform (Analytic Sale Module)

DEPRECATED=	Outdated, uses EOLed python27
EXPIRATION_DATE=	2020-02-03

LICENSE=	GPLv3

RUN_DEPENDS=	trytond28_analytic_account>=2.8.0:finance/trytond28_analytic_account \
		trytond28_analytic_invoice>=2.8.0:finance/trytond28_analytic_invoice \
		trytond28_sale>=2.8.1:finance/trytond28_sale

CONFLICTS=	trytond_analytic_sale-2.[46].*

USES=		python:2.7
USE_PYTHON=	distutils autoplist

.include <bsd.port.mk>
