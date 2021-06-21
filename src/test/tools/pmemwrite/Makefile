# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2021, Intel Corporation
#
# Makefile -- Makefile for pmemwrite tool
#

TOP = ../../../..

TARGET = pmemwrite

OBJS = write.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEMBLK)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEMLOG)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEM)

TOOLS_COMMON=y

include $(TOP)/src/tools/Makefile.inc
