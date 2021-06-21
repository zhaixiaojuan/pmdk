# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2017-2021, Intel Corporation
#
# Makefile -- Makefile for cmpmap tool
#

TOP = ../../../..

TARGET = cmpmap
OBJS = cmpmap.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM)

LIBPMEMCOMMON=y

include $(TOP)/src/tools/Makefile.inc
