#	$OpenBSD: Makefile,v 1.1 2017/01/24 08:50:57 beck Exp $

PROG=	ocspcheck
MAN=	ocspcheck.8

LDADD=	-ltls -lssl -lcrypto
DPADD=	${LIBTLS} ${LIBSSL} ${LIBCRYPTO}

CFLAGS+= -Wall -Werror
CFLAGS+= -Wformat
CFLAGS+= -Wformat-security
CFLAGS+= -Wimplicit
CFLAGS+= -Wreturn-type
CFLAGS+= -Wshadow
CFLAGS+= -Wtrigraphs
CFLAGS+= -Wuninitialized
CFLAGS+= -Wunused

CFLAGS+= -DLIBRESSL_INTERNAL

SRCS=	ocspcheck.c http.c

.include <bsd.prog.mk>
