# $NetBSD: Makefile,v 1.27 2021/05/23 08:12:13 taca Exp $

DISTNAME=	tiny_tds-2.1.5
PKGNAME=	${RUBY_PKGPREFIX}-${DISTNAME}
CATEGORIES=	databases

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/rails-sqlserver/tiny_tds
COMMENT=	Modern, simple and fast FreeTDS library for Ruby using DB-Library
LICENSE=	mit

DEPENDS+=	${RUBY_PKGPREFIX}-mini_portile2>=2.0<3:../../misc/ruby-mini_portile2

# No ALTERNATIVES file since bin/defncopy and bin/tsql conflict
# with freetds.
RUBYGEM_OPTIONS+=	--format-executable

.include "../../databases/freetds/buildlink3.mk"
.include "../../lang/ruby/gem.mk"
.include "../../mk/bsd.pkg.mk"
