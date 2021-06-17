# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2016-2021, Intel Corporation
#
# Makefile -- Makefile for pmemdetect tool
#

TOP = ../../../..

TARGET = pmemdetect

OBJS = pmemdetect.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMBLK_OBJS_NONDEBUG)
endif

TOOLS_COMMON=y

SCP_TO_REMOTE_NODES = y

include $(TOP)/src/tools/Makefile.inc
