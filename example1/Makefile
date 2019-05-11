ifneq ($(KERNELRELEASE),)
obj-m := hello.o
else
    
KDIR := /lib/modules/4.18.0-18-generic/build
all:
	make -C $(KDIR) M=$(PWD) modules
clean:
	rm -f *.ko *.o *.mod.o *.mod.c *.symvers
endif
