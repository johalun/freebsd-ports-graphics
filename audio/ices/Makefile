# Created by: Michael Nottebrock <michaelnottebrock@gmx.net>
# $FreeBSD$

PORTNAME=	ices
PORTVERSION=	2.0.2
PORTREVISION=	2
PORTEPOCH=	1
CATEGORIES=	audio net
MASTER_SITES=	http://downloads.xiph.org/releases/${PORTNAME}/ \
		http://svn.xiph.org/releases/${PORTNAME}/

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Vorbis streaming source client for icecast 2

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/COPYING

LIB_DEPENDS=	libogg.so:audio/libogg \
		libshout.so:audio/libshout \
		libspeex.so:audio/speex \
		libtheora.so:multimedia/libtheora \
		libvorbis.so:audio/libvorbis

OPTIONS_DEFINE=	ALSA

CONFIGURE_ARGS=	--disable-roaraudio --disable-sun-audio
GNU_CONFIGURE=	yes
USE_GNOME=	libxml2
USES=		gmake iconv pkgconfig tar:bzip2

PLIST_FILES=	bin/ices
PORTDATA=	*

ALSA_LIB_DEPENDS=	libasound.so:audio/alsa-lib
ALSA_CONFIGURE_ENABLE=	alsa

.include <bsd.port.mk>
