# $NetBSD: Makefile,v 1.31 2021/05/20 13:53:28 tonio Exp $

DISTNAME=	hevea-2.35
CATEGORIES=	textproc
MASTER_SITES=	http://hevea.inria.fr/distri/

MAINTAINER=	tonio@NetBSD.org
HOMEPAGE=	http://hevea.inria.fr/
COMMENT=	LaTeX to HTML translator
LICENSE=	qpl-v1.0

MAKE_ENV+=	DESTDIR=${DESTDIR}

.include "../../mk/ocaml.mk"
.if !empty(OCAML_USE_OPT_COMPILER:M[Yy][Ee][Ss])
MAKE_ENV+=	TARGET=opt
.else
MAKE_ENV+=	TARGET=byte
.endif

.include "../../devel/ocamlbuild/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
