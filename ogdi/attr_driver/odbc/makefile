#
# Copyright (C) 1997 Logiciels et Applications Scientifiques (L.A.S.) Inc
# Permission to use, copy, modify and distribute this software and
# its documentation for any purpose and without fee is hereby granted,
# provided that the above copyright notice appear in all copies, that
# both the copyright notice and this permission notice appear in
# supporting documentation, and that the name of L.A.S. Inc not be used 
# in advertising or publicity pertaining to distribution of the software 
# without specific, written prior permission. L.A.S. Inc. makes no
# representations about the suitability of this software for any purpose.
# It is provided "as is" without express or implied warranty.
#

TOBEGEN	= lodbc
TARGETGEN=$(DYNAGEN)

SOURCES = odbc.c

INCLUDES = $(CURRENT_INCLUDE) $(GENERAL_INCLUDE) \
	   $(OGDI_INCLUDE) $(PROJ_INCLUDE)
CFLAGS 	= $(INCLUDES) $(COMMON_CFLAGS)

LINK_LIBS= $(ODBC_LINKLIB)

include $(TOPDIR)/config/common.mak

all: MKOBJECTDIR 
	$(MAKE) --directory $(OBJDIR) -f ../makefile PASS='depend' $(TARGETGEN)

clean: default-clean
