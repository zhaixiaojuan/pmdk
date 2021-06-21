# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2018-2021, Intel Corporation

#
# src/test/tools/obj_verify -- build obj_verify tool
#

SCP_TO_REMOTE_NODES = y

TOP = ../../../..

TARGET = obj_verify
OBJS = obj_verify.o

OBJS += $(call lib_objs,$(BUILDTYPE),PMEM)
OBJS += $(call lib_objs,$(BUILDTYPE),PMEMOBJ)

LIBPMEMCOMMON=y

include $(TOP)/src/tools/Makefile.inc
