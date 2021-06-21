# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2019-2021, Intel Corporation
#
# Makefile -- Makefile for gran_detecto tool
#

TOP = ../../../..

include $(TOP)/src/common.inc

INCS += -I$(TOP)/src/core
INCS += -I$(TOP)/src/common

TARGET = gran_detecto

OBJS += gran_detecto.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM2)
OBJS += $(subst /libpmemcore/,/core/,$(call lib_objs,$(BUILDTYPE),PMEMCORE))

CFLAGS += $(LIBNDCTL_CFLAGS)
LIBS += $(LIBNDCTL_LIBS) -pthread

include $(TOP)/src/tools/Makefile.inc
