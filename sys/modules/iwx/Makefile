# $FreeBSD$

.PATH:  ${.CURDIR}/../../dev/iwx
CFLAGS+=	-I${.CURDIR}/../..

KMOD=	if_iwx
SRCS=	if_iwx.c
SRCS+=	device_if.h bus_if.h pci_if.h opt_wlan.h opt_iwm.h

CFLAGS+= -DIWX_DEBUG
DEBUG_FLAGS=	-O0 -g

.include <bsd.kmod.mk>
