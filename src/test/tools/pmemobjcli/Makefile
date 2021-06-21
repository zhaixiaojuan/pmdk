# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2021, Intel Corporation
#
# Makefile -- Makefile for pmemalloc tool
#

TOP=../../../..

SCP_TO_REMOTE_NODES = y

TARGET = pmemobjcli

OBJS = pmemobjcli.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEMOBJ)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEMBLK)

TOOLS_COMMON=y

include $(TOP)/src/tools/Makefile.inc
