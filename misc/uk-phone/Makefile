PORTNAME=	uk-phone
PORTVERSION=	2.7
CATEGORIES=	misc
MASTER_SITES=	ftp://ftp.Awfulhak.org/pub/uk-phone/ \
		http://people.FreeBSD.org/~brian/uk-phone/
EXTRACT_SUFX=	.gz

MAINTAINER=	ports@FreeBSD.org
COMMENT=	United Kingdom phone codes

DEPRECATED=	Obsolete, 20+ year old data
EXPIRATION_DATE=2024-10-31

NO_WRKSUBDIR=	yes
EXTRACT_CMD=	${GZCAT}
EXTRACT_BEFORE_ARGS=	# None
EXTRACT_AFTER_ARGS=	> ${WRKSRC}/uk.phone
NO_BUILD=	yes
PLIST_FILES=	share/misc/uk.phone

do-install:
	${INSTALL_DATA} ${WRKSRC}/uk.phone ${STAGEDIR}${PREFIX}/share/misc

.include <bsd.port.mk>
