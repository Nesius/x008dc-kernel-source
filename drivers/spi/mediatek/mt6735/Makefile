subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/include/mt-plat/$(MTK_PLATFORM)/include \
					-I$(srctree)/drivers/misc/mediatek/include/mt-plat
ifeq ($(CONFIG_TRUSTONIC_TEE_SUPPORT),y)
subdir-ccflags-y += -I$(srctree)/drivers/spi/trustzone/spi/Tlspi/inc
endif

ifeq ($(CONFIG_TRUSTONIC_TEE_SUPPORT),y)
	include $(srctree)/drivers/misc/mediatek/gud/Makefile.include
endif
# dingyisheng@wind-mobi.com 20161115 begin
ifeq ($(CONFIG_TRUSTKERNEL_TEE_SUPPORT),y)
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/tkcore/include/linux
endif
# dingyisheng@wind-mobi.com 20161115 end
obj-$(CONFIG_MTK_SPI) += spi.o spi-dev.o
