# SPDX-License-Identifier: GPL-2.0-only
#
# Copyright (C) 2017-2021 OpenWrt.org

include $(TOPDIR)/rules.mk

ARCH:=mipsel
BOARD:=pistachio
BOARDNAME:=MIPS pistachio
FEATURES:=fpu usb usbgadget squashfs targz nand
CPU_TYPE:=24kc
CPU_SUBTYPE:=24kf
SUBTARGETS:=generic

KERNEL_PATCHVER:=6.12

include $(INCLUDE_DIR)/target.mk

KERNELNAME:=vmlinux dtbs

DEFAULT_PACKAGES += \
	kmod-gpio-button-hotplug \
	uboot-envtools

$(eval $(call BuildTarget))
