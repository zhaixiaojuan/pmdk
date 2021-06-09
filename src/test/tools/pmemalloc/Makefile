# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2017, Intel Corporation
#
# Makefile -- Makefile for pmemalloc tool
#

TOP = ../../../..

TARGET = pmemalloc

OBJS = pmemalloc.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
	OBJS += $(LIBPMEMOBJ_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMOBJ_OBJS_NONDEBUG)
endif

LIBPMEMCOMMON=y

include $(TOP)/src/tools/Makefile.inc
