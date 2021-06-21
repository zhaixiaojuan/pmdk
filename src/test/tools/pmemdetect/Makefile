# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2016-2021, Intel Corporation
#
# Makefile -- Makefile for pmemdetect tool
#

TOP = ../../../..

TARGET = pmemdetect

OBJS = pmemdetect.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEMBLK)

TOOLS_COMMON=y

SCP_TO_REMOTE_NODES = y

include $(TOP)/src/tools/Makefile.inc
