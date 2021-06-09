# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2016, Intel Corporation
#
# Makefile -- Makefile for pmemspoil tool
#

TOP=../../../..

SCP_TO_REMOTE_NODES = y

TARGET = pmemspoil

OBJS = spoil.o

TOOLS_COMMON=y

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_NONDEBUG)
endif

include $(TOP)/src/tools/Makefile.inc
