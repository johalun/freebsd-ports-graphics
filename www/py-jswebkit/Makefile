# Created by: Ju Pengfei <jupengfei@gmail.com>
# $FreeBSD$

PORTNAME=	jswebkit
PORTVERSION=	0.0.3
PORTREVISION=	4
CATEGORIES=	www python
MASTER_SITES=	http://archive.ubuntu.com/ubuntu/pool/universe/p/python-jswebkit/
PROJECTHOST=	gwrite
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
DISTNAME=	python-${PORTNAME}_${PORTVERSION}.orig

MAINTAINER=	ports@FreeBSD.org
COMMENT=	WebKit/JavaScriptCore Python bindings

BUILD_DEPENDS=	cython:lang/cython
RUN_DEPENDS:=	${BUILD_DEPENDS}
LIB_DEPENDS=	libwebkitgtk-1.0.so:www/webkit-gtk2

USES=		pkgconfig python:2
USE_PYTHON=	distutils autoplist
WRKSRC=		${WRKDIR}/python-${PORTNAME}-${PORTVERSION}

post-install:
	${STRIP_CMD} ${STAGEDIR}${PYTHONPREFIX_SITELIBDIR}/jswebkit.so

.include <bsd.port.mk>
