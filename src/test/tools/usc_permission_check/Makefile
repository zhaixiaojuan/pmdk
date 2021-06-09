# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2018-2020, Intel Corporation
#
# Makefile -- Makefile for fallocate detection tool
#

TOP = ../../../..

TARGET = usc_permission_check
OBJS = usc_permission_check.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM2_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM2_OBJS_NONDEBUG)
endif
LIBPMEMCORE=y
include $(TOP)/src/tools/Makefile.inc
