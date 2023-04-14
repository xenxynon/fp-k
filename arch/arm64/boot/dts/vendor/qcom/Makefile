ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)

dtbo-$(CONFIG_ARCH_LAGOON) += \
		lagoon-mtp-overlay_fp4.dtbo

lagoon-mtp-overlay_fp4.dtbo-base := lagoon.dtb

else
$(error Builds without CONFIG_BUILD_ARM64_DT_OVERLAY are not supported. In Android builds this is enabled from device/qcom/kernelscripts/kernel_definitions.mk)
endif

always		:= $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
