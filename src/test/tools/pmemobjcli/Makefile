# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2021, Intel Corporation
#
# Makefile -- Makefile for pmemalloc tool
#

TOP=../../../..

SCP_TO_REMOTE_NODES = y

TARGET = pmemobjcli

OBJS = pmemobjcli.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
	OBJS += $(LIBPMEMOBJ_OBJS_DEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMOBJ_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_NONDEBUG)
endif

TOOLS_COMMON=y

include $(TOP)/src/tools/Makefile.inc
