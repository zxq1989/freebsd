# $FreeBSD$
# $Whistle: Makefile,v 1.2 1999/01/19 19:39:21 archie Exp $

KMOD=	ng_iface
SRCS= 	ng_iface.c opt_inet.h opt_inet6.h

.if !defined(KERNBUILDDIR)
opt_inet.h:
	echo "#define INET 1" > ${.TARGET}

opt_inet6.h:
	echo "#define INET6 1" > ${.TARGET}
.endif

.include <bsd.kmod.mk>
