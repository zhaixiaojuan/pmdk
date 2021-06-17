# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2018-2021, Intel Corporation

#
# src/test/tools/obj_verify -- build obj_verify tool
#

SCP_TO_REMOTE_NODES = y

TOP = ../../../..

TARGET = obj_verify
OBJS = obj_verify.o

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
	OBJS += $(LIBPMEMOBJ_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
	OBJS += $(LIBPMEMOBJ_OBJS_NONDEBUG)
endif

LIBPMEMCOMMON=y

include $(TOP)/src/tools/Makefile.inc
