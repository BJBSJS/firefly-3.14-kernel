dtb-$(CONFIG_ARCH_VEXPRESS) += rtsm_ve-aemv8a.dtb foundation-v8.dtb
dtb-$(CONFIG_ARCH_XGENE) += apm-mustang.dtb
dtb-$(CONFIG_ARCH_TEGRA) += tegra132-norrin.dtb
dtb-$(CONFIG_ARCH_TEGRA) += tegra132-ryu-p1.dtb
dtb-$(CONFIG_ARCH_TEGRA) += tegra132-ryu-p3.dtb
dtb-$(CONFIG_ARCH_TEGRA) += tegra132-ryu-p4.dtb

DTB_NAMES := $(subst $\",,$(CONFIG_BUILD_ARM64_APPENDED_DTB_IMAGE_NAMES))
ifneq ($(DTB_NAMES),)
DTB_LIST := $(addsuffix .dtb,$(DTB_NAMES))
else
DTB_LIST := $(dtb-y)
endif

always		:= $(DTB_LIST)
clean-files := dts/*.dtb *.dtb
