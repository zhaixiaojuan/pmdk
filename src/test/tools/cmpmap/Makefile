# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2017-2021, Intel Corporation
#
# Makefile -- Makefile for cmpmap tool
#

TOP = ../../../..

TARGET = cmpmap
OBJS = cmpmap.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
endif

LIBPMEMCOMMON=y

include $(TOP)/src/tools/Makefile.inc
