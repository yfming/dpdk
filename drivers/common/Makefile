# SPDX-License-Identifier: BSD-3-Clause
# Copyright(c) 2018 Cavium, Inc
#

include $(RTE_SDK)/mk/rte.vars.mk

ifeq ($(CONFIG_RTE_LIBRTE_PMD_OCTEONTX_SSOVF)$(CONFIG_RTE_LIBRTE_OCTEONTX_MEMPOOL),yy)
DIRS-y += octeontx
endif

MVEP-y := $(CONFIG_RTE_LIBRTE_MVPP2_PMD)
MVEP-y += $(CONFIG_RTE_LIBRTE_MVNETA_PMD)
ifneq (,$(findstring y,$(MVEP-y)))
DIRS-y += mvep
endif

include $(RTE_SDK)/mk/rte.subdir.mk
