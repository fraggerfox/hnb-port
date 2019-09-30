# Created by: Patrick Li <pat@databits.net>
# $FreeBSD: head/editors/hnb/Makefile 405891 2016-01-12 16:20:31Z amdmi3 $

PORTNAME=	hnb
PORTVERSION=	1.9.18
DISTVERSIONPREFIX=	v
CATEGORIES=	editors

MAINTAINER=	amdmi3@FreeBSD.org
COMMENT=	Hierarchical NoteBook a data organizer

LICENSE=	GPLv2+
LICENSE_FILE=	${WRKSRC}/COPYING

USES=		gmake

USE_GITHUB=	yes
GH_ACCOUNT=	fraggerfox

MAKE_JOBS_UNSAFE=	yes

PLIST_FILES=	bin/${PORTNAME} \
		man/man1/${PORTNAME}.1.gz
PORTDOCS=	*

OPTIONS_DEFINE=	DOCS

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/src/hnb ${STAGEDIR}${PREFIX}/bin
	${INSTALL_MAN}	${WRKSRC}/doc/hnb.1 ${STAGEDIR}${MAN1PREFIX}/man/man1
	${MKDIR} ${STAGEDIR}${DOCSDIR}
.for FILE in Documentation.hnb Documentation.html hnbrc
	${INSTALL_DATA} ${WRKSRC}/doc/${FILE} ${STAGEDIR}${DOCSDIR}
.endfor

.include <bsd.port.mk>
