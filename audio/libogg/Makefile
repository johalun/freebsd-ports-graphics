# Created by: t.vanklaveren@student.utwente.nl
# $FreeBSD$

PORTNAME=	libogg
PORTVERSION=	1.3.2
PORTREVISION=	1
PORTEPOCH=	4
CATEGORIES=	audio
MASTER_SITES=	http://downloads.xiph.org/releases/ogg/

MAINTAINER=	naddy@FreeBSD.org
COMMENT=	Ogg bitstream library

USES=		libtool pathfix tar:xz
USE_LDCONFIG=	yes
GNU_CONFIGURE=	yes
INSTALL_TARGET=	install-strip
TEST_TARGET=	check

OPTIONS_DEFINE=	DOCS

post-stage:
	${LN} -s libogg.so.0 ${STAGEDIR}${PREFIX}/lib/libogg.so.8

.include <bsd.port.mk>
