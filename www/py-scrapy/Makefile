# Created by: Qing Feng <qingfeng@douban.com>
# $FreeBSD$

PORTNAME=	Scrapy
PORTVERSION=	1.3.3
PORTREVISION=	1
CATEGORIES=	www python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	skreuzer@FreeBSD.org
COMMENT=	High level scraping and web crawling framework

LICENSE=	BSD3CLAUSE

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}twisted>=15.5.0:devel/py-twisted@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}lxml>=3.2.4:devel/py-lxml@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}sqlite3>0:databases/py-sqlite3@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}w3lib>=1.14.2:www/py-w3lib@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}cssselect>=0.9:www/py-cssselect@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}queuelib>=1.2.2:sysutils/py-queuelib@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pydispatcher>=2.0.5:devel/py-pydispatcher@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}service_identity>0:security/py-service_identity@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}parsel>=1.1:textproc/py-parsel@${FLAVOR}

USES=		python
USE_PYTHON=	distutils autoplist

OPTIONS_DEFINE=	SSL
OPTIONS_DEFAULT=SSL

.include <bsd.port.options.mk>

.if ${PORT_OPTIONS:MSSL}
RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}openssl>0:security/py-openssl@${FLAVOR}
.endif

.include <bsd.port.mk>
