obj-m += kbdm.o
CURRENT_PATH := $(shell pwd)
LINUX_KERNEL := $(shell uname -r)
LINUX_KERNEL_PATH := /usr/src/linux-headers-$(LINUX_KERNEL)
all:
	make -C $(LINUX_KERNEL_PATH) M=$(CURRENT_PATH) modules
#-C表示在编译前更改目录
#M=dir指定寻找编译内容的位置
#modules 说明编译为内核模块
clean:
	make -C $(LINUX_KERNEL_PATH) M=$(CURRENT_PATH) clean
