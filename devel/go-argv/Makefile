# $NetBSD: Makefile,v 1.18 2021/06/06 12:18:48 bsiegert Exp $

GITHUB_TAG=	v${PKGVERSION_NOREV}
DISTNAME=	go-argv-0.0.1
PKGREVISION=	16
CATEGORIES=	devel
MASTER_SITES=	${MASTER_SITE_GITHUB:=cosiner/}
GITHUB_PROJECT=	argv

MAINTAINER=	nikita@NetBSD.org
HOMEPAGE=	https://github.com/cosiner/argv
COMMENT=	Go library to split command line string into arguments array
LICENSE=	mit

GO_SRCPATH=	github.com/cosiner/argv
GO_DIST_BASE=	argv-${PKGVERSION_NOREV}

.include "../../lang/go/go-package.mk"
.include "../../mk/bsd.pkg.mk"
