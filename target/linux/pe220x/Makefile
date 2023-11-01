# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

BOARD:=pe220x
BOARDNAME:=Phytium PE220x
FEATURES:=ext4 audio usb usbgadget display gpio fpu pci pcie rootfs-part boot-part squashfs
SUBTARGETS:=armv8

KERNEL_PATCHVER=5.10

define Target/Description
	Build firmware image for PE220x SoC devices.
endef

include $(INCLUDE_DIR)/target.mk

DEFAULT_PACKAGES += uboot-envtools partx-utils e2fsprogs mkf2fs

KERNELNAME:=Image dtbs

$(eval $(call BuildTarget))
