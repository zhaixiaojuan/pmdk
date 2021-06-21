# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2021, Intel Corporation
#
# Makefile -- Makefile for pmemalloc tool
#

TOP = ../../../..

TARGET = pmemalloc

OBJS = pmemalloc.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEMOBJ)

LIBPMEMCOMMON=y

include $(TOP)/src/tools/Makefile.inc
