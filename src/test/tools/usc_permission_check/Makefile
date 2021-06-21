# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2018-2021, Intel Corporation
#
# Makefile -- Makefile for fallocate detection tool
#

TOP = ../../../..

TARGET = usc_permission_check
OBJS = usc_permission_check.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM2)

LIBPMEMCORE=y
include $(TOP)/src/tools/Makefile.inc
