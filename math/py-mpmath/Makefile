# $NetBSD: Makefile,v 1.16 2021/05/12 08:32:16 adam Exp $

DISTNAME=	mpmath-1.2.1
PKGNAME=	${PYPKGPREFIX}-${DISTNAME}
CATEGORIES=	math python
MASTER_SITES=	${MASTER_SITE_PYPI:=m/mpmath/}
MASTER_SITES+=	http://mpmath.org/files/

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://mpmath.org/
COMMENT=	Python library for arbitrary-precision FP arithmetic
LICENSE=	modified-bsd

BUILD_DEPENDS+=	${PYPKGPREFIX}-setuptools_scm-[0-9]*:../../devel/py-setuptools_scm
# py-gmpy provides faster backend
DEPENDS+=	${PYPKGPREFIX}-gmpy-[0-9]*:../../math/py-gmpy
TEST_DEPENDS+=	${PYPKGPREFIX}-test-runner-[0-9]*:../../devel/py-test-runner

USE_LANGUAGES=	# none

PYSETUPTESTTARGET=	pytest

.include "../../lang/python/egg.mk"
.include "../../mk/bsd.pkg.mk"
