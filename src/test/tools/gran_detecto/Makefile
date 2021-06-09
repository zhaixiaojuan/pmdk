# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2019-2020, Intel Corporation
#
# Makefile -- Makefile for gran_detecto tool
#

TOP = ../../../..

include $(TOP)/src/common.inc

INCS += -I$(TOP)/src/core
INCS += -I$(TOP)/src/common

TARGET = gran_detecto

OBJS += gran_detecto.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM2_OBJS_DEBUG)
	OBJS += $(LIBPMEMCORE_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM2_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMCORE_OBJS_NONDEBUG)
endif

CFLAGS += $(LIBNDCTL_CFLAGS)
LIBS += $(LIBNDCTL_LIBS) -pthread

include $(TOP)/src/tools/Makefile.inc
