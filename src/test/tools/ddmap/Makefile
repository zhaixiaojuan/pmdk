# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2021, Intel Corporation
#
# Makefile -- Makefile for ddmap tool
#

TOP = ../../../..

TARGET = ddmap

OBJS = ddmap.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEMBLK)

TOOLS_COMMON=y

include $(TOP)/src/tools/Makefile.inc
