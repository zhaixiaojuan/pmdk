# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2016, Intel Corporation
#
# Makefile -- Makefile for bttcreate tool
#
TOP = ../../../..

vpath %.c $(TOP)/src/libpmemblk/

TARGET = bttcreate
OBJS = bttcreate.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_NONDEBUG)
endif

LIBPMEMCOMMON=y

include $(TOP)/src/tools/Makefile.inc
INCS += -I$(TOP)/src/libpmemblk
