##
## This file is part of the libopencm3 project.
##
## Copyright (C) 2012 Alexandru Gagniuc <mr.nuke.me@gmail.com>
##
## This library is free software: you can redistribute it and/or modify
## it under the terms of the GNU Lesser General Public License as published by
## the Free Software Foundation, either version 3 of the License, or
## (at your option) any later version.
##
## This library is distributed in the hope that it will be useful,
## but WITHOUT ANY WARRANTY; without even the implied warranty of
## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
## GNU Lesser General Public License for more details.
##
## You should have received a copy of the GNU Lesser General Public License
## along with this library.  If not, see <http://www.gnu.org/licenses/>.
##

BINARY          = tomu-runner
OBJS            = usb-cdcacm.o

LIBNAME         = opencm3_efm32hg
DEFS            += -DEFM32HG

FP_FLAGS        ?= -mfloat-abi=soft
ARCH_FLAGS      = -mthumb -mcpu=cortex-m0plus $(FP_FLAGS)
DEFS            += -I.

LDSCRIPT        = tomu-efm32hg309.ld
LIBPATHS        = ./libopencm3
OPENCM3_DIR     = libopencm3

include libopencm3_rules.mk
