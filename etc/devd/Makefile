# $FreeBSD$

.include <bsd.own.mk>

FILES=	uath.conf usb.conf

.if ${MACHINE} == "powerpc"
FILES+=	apple.conf
.endif

.if ${MACHINE} == "amd64" || ${MACHINE} == "i386"
FILES+=	asus.conf
.endif

.if ${MK_HYPERV} != "no"
FILES+=	hyperv.conf
.endif

NO_OBJ=
FILESDIR=	/etc/devd
FILESMODE=	644

.include <bsd.prog.mk>
