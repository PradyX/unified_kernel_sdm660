# SPDX-License-Identifier: GPL-2.0

ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
dtbo-$(CONFIG_ARCH_SDM660) += \
	sdm660-mtp-jasmine-overlay.dtbo \
	sdm660-mtp-wayne-overlay.dtbo

sdm660-mtp-jasmine-overlay.dtbo-base := sdm660-mtp-jasmine.dtb
sdm660-mtp-wayne-overlay.dtbo-base := sdm660-mtp-wayne.dtb
else
dtb-$(CONFIG_ARCH_SDM660) += \
	sdm660-mtp-jasmine.dtb \
	sdm660-mtp-wayne.dtb
endif

always		:= $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
