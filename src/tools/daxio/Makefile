# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2018-2021, Intel Corporation
#
# Makefile -- top Makefile for daxio
#

TOP = ../../..
include $(TOP)/src/common.inc

ifeq ($(NDCTL_ENABLE),y)

SCP_TO_REMOTE_NODES = y

TARGET = daxio
OBJS = daxio.o

LIBPMEMCOMMON=y

ifneq ($(DEBUG),)
	OBJS += $(LIBPMEM_OBJS_DEBUG)
else
	OBJS += $(LIBPMEM_OBJS_NONDEBUG)
endif

CFLAGS += $(LIBNDCTL_CFLAGS)
LIBS += $(LIBNDCTL_LIBS)

MANPAGES = $(TOP)/doc/daxio.1

# XXX: to be done
# BASH_COMP_FILES = daxio.sh

else
$(info NOTE: Skipping daxio because ndctl is not available)
endif

include ../Makefile.inc

.PHONY: test check
