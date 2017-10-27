ccflags-y += -Idrivers/media/platform/msm/camera_v2
ccflags-y += -Idrivers/media/platform/msm/camera_v2/sensor
ccflags-y += -Idrivers/media/platform/msm/camera_v2/sensor-trunk
ccflags-y += -Idrivers/media/platform/msm/camera_v2/codecs
ccflags-y += -Idrivers/media/platform/msm/camera_v2/isps
ccflags-y += -Idrivers/media/platform/msm/camera_v2/pproc
ccflags-y += -Idrivers/media/platform/msm/camera_v2/msm_vb2
ccflags-y += -Idrivers/media/platform/msm/camera_v2/camera
ccflags-y += -Idrivers/media/platform/msm/camera_v2/jpeg_10
ccflags-y += -Idrivers/media/platform/msm/camera_v2/fd

obj-$(CONFIG_MSMB_CAMERA) += msm.o
obj-$(CONFIG_MSMB_CAMERA) += camera/
obj-$(CONFIG_MSMB_CAMERA) += msm_vb2/
ifeq ($(CONFIG_MACH_TRUNK),y)
obj-$(CONFIG_MSMB_CAMERA) += sensor-trunk/
else
obj-$(CONFIG_MSMB_CAMERA) += sensor/
endif # MACH_TRUNK
obj-$(CONFIG_MSMB_CAMERA) += pproc/
ifeq ($(CONFIG_MACH_TRUNK),y)
obj-$(CONFIG_MSMB_CAMERA) += isp-trunk/
else
obj-$(CONFIG_MSMB_CAMERA) += isp/
endif # MACH_TRUNK
obj-$(CONFIG_MSMB_CAMERA) += ispif/
obj-$(CONFIG_MSMB_JPEG) += jpeg_10/
obj-$(CONFIG_MSMB_CAMERA) += msm_buf_mgr/
obj-$(CONFIG_MSM_FD) += fd/
