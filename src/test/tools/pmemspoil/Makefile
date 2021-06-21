# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2021, Intel Corporation
#
# Makefile -- Makefile for pmemspoil tool
#

TOP=../../../..

SCP_TO_REMOTE_NODES = y

TARGET = pmemspoil

OBJS = spoil.o

TOOLS_COMMON=y

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEMBLK)

include $(TOP)/src/tools/Makefile.inc
