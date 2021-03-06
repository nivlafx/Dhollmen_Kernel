#
# Makefile for the Linux kernel device drivers.
#
# 15 Sep 2000, Christoph Hellwig <hch@infradead.org>
# Rewritten to use lists instead of if-statements.
#

obj-y				+= gpio/
obj-$(CONFIG_RAPIDIO)		+= rapidio/
obj-y				+= video/
obj-y				+= idle/
obj-$(CONFIG_SFI)		+= sfi/
obj-$(CONFIG_DMA_ENGINE)	+= dma/
obj-$(CONFIG_VIRTIO)		+= virtio/
obj-$(CONFIG_RPMSG)		+= rpmsg/
obj-$(CONFIG_REGULATOR)		+= regulator/
obj-y				+= tty/
obj-y				+= char/
obj-y				+= gpu/
obj-$(CONFIG_CONNECTOR)		+= connector/
obj-y				+= base/ block/ misc/ mfd/
obj-$(CONFIG_NUBUS)		+= nubus/
obj-$(CONFIG_SCSI)		+= scsi/
obj-$(CONFIG_TARGET_CORE)	+= target/
obj-$(CONFIG_MTD)		+= mtd/
obj-$(CONFIG_SPI)		+= spi/
obj-y				+= net/
obj-y				+= cdrom/
obj-$(CONFIG_DIO)		+= dio/
obj-$(CONFIG_SBUS)		+= sbus/
obj-$(CONFIG_ZORRO)		+= zorro/
obj-$(CONFIG_ATA_OVER_ETH)	+= block/aoe/
obj-$(CONFIG_TC)		+= tc/
obj-$(CONFIG_USB_OTG_UTILS)	+= usb/
obj-$(CONFIG_USB)		+= usb/
obj-$(CONFIG_USB_GADGET)	+= usb/
obj-$(CONFIG_SERIO)		+= input/serio/
obj-$(CONFIG_GAMEPORT)		+= input/gameport/
obj-$(CONFIG_INPUT)		+= input/
obj-$(CONFIG_RTC_LIB)		+= rtc/
obj-y				+= i2c/ media/
obj-$(CONFIG_PPS)		+= pps/
obj-$(CONFIG_PTP_1588_CLOCK)	+= ptp/
obj-$(CONFIG_W1)		+= w1/
obj-$(CONFIG_POWER_SUPPLY)	+= power/
obj-$(CONFIG_HWMON)		+= hwmon/
obj-$(CONFIG_THERMAL)		+= thermal/
obj-$(CONFIG_WATCHDOG)		+= watchdog/
obj-$(CONFIG_MD)		+= md/
obj-$(CONFIG_BT)		+= bluetooth/
obj-y				+= lguest/
obj-$(CONFIG_CPU_FREQ)		+= cpufreq/
obj-$(CONFIG_CPU_IDLE)		+= cpuidle/
obj-$(CONFIG_MMC)		+= mmc/
obj-$(CONFIG_MEMSTICK)		+= memstick/
obj-y				+= leds/
obj-$(CONFIG_SWITCH)		+= switch/
obj-$(CONFIG_SGI_SN)		+= sn/
obj-y				+= firmware/
obj-$(CONFIG_CRYPTO)		+= crypto/
obj-$(CONFIG_SUPERH)		+= sh/
obj-$(CONFIG_ARCH_SHMOBILE)	+= sh/
ifndef CONFIG_ARCH_USES_GETTIMEOFFSET
obj-y				+= clocksource/
endif
obj-$(CONFIG_HID)		+= hid/
obj-$(CONFIG_PPC_PS3)		+= ps3/
obj-$(CONFIG_OF)		+= of/
obj-$(CONFIG_SSB)		+= ssb/
obj-$(CONFIG_BCMA)		+= bcma/
obj-$(CONFIG_VHOST_NET)		+= vhost/
obj-$(CONFIG_VLYNQ)		+= vlynq/
obj-$(CONFIG_STAGING)		+= staging/
obj-y				+= clk/

obj-$(CONFIG_HWSPINLOCK)	+= hwspinlock/
obj-$(CONFIG_REMOTE_PROC)	+= remoteproc/

obj-$(CONFIG_DMM_OMAP)		+= media/
obj-$(CONFIG_TILER_OMAP)	+= media/
obj-$(CONFIG_SAMSUNG_MODULES) 	+= samsung/
obj-$(CONFIG_OMAP_HSI)		+= omap_hsi/
obj-$(CONFIG_INPUT_YAS_SENSORS)	+= sensors/
obj-$(CONFIG_SAMSUNG_PHONE_SVNET) += modemctl/
obj-$(CONFIG_PHONE_IPC_SPI) 	+= phone_svn/
obj-$(CONFIG_BATTERY_SAMSUNG)   += battery/

ifeq (1, $(shell if [ -d $(srctree)/drivers/exfat ]; then echo 1; fi))
obj-$(CONFIG_SAMSUNG_EXFAT)	+= exfat/
endif
