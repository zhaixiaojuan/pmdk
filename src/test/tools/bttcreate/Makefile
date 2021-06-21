# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2016-2021, Intel Corporation
#
# Makefile -- Makefile for bttcreate tool
#
TOP = ../../../..

vpath %.c $(TOP)/src/libpmemblk/

TARGET = bttcreate
OBJS = bttcreate.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEMBLK)

LIBPMEMCOMMON=y

include $(TOP)/src/tools/Makefile.inc
INCS += -I$(TOP)/src/libpmemblk
