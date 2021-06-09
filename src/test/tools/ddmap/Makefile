# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2016, Intel Corporation
#
# Makefile -- Makefile for ddmap tool
#

TOP = ../../../..

TARGET = ddmap

OBJS = ddmap.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_NONDEBUG)
endif

TOOLS_COMMON=y

include $(TOP)/src/tools/Makefile.inc
