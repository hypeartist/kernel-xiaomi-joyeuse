MODNAME = qdsp6v2
AUDIO_ROOT := $(srctree)/drivers/audio/qcom

include $(AUDIO_ROOT)/config/atollauto.conf
export

# Use USERINCLUDE when you must reference the UAPI directories only.
USERINCLUDE     += \
                -I$(AUDIO_ROOT)/include/uapi \

# Use LINUXINCLUDE when you must reference the include/ directory.
# Needed to be compatible with the O= option
LINUXINCLUDE    += \
                -I$(AUDIO_ROOT)/include/uapi \
                -I$(AUDIO_ROOT)/include

LINUXINCLUDE    += \
                -include $(AUDIO_ROOT)/config/atollautoconf.h

obj-y += soc/
obj-y += dsp/
obj-y += dsp/elliptic/
obj-y += ipc/
obj-y += asoc/
