# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2021, Intel Corporation
#
# Makefile -- Makefile for pmemwrite tool
#

TOP = ../../../..

TARGET = pmemwrite

OBJS = write.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEMBLK_OBJS_DEBUG)
	OBJS += $(LIBPMEMLOG_OBJS_DEBUG)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
else
	OBJS += $(LIBPMEMBLK_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMLOG_OBJS_NONDEBUG)
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
endif

TOOLS_COMMON=y

include $(TOP)/src/tools/Makefile.inc
