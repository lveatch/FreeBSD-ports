# Created by: Cyrille Lefevre <cyrille.lefevre@laposte.net>
# $FreeBSD$

PORTNAME=	gzip
PORTVERSION=	1.9
CATEGORIES=	archivers
MASTER_SITES=	GNU

MAINTAINER=	johans@FreeBSD.org
COMMENT=	Compression utility designed to be a replacement for compress

LICENSE=	GPLv3+

USES=		cpe charsetfix makeinfo
GNU_CONFIGURE=	yes

INFO=		gzip
CPE_VENDOR=	gnu

DOC_FILES=	AUTHORS COPYING ChangeLog ChangeLog-2007 INSTALL NEWS README \
		THANKS TODO

OPTIONS_DEFINE=	DOCS

post-install:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	cd ${WRKSRC} && ${INSTALL_DATA} ${DOC_FILES} ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>
