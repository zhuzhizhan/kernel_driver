BASEINCLUDE ?= /home/zzz/code/kernel_driver/example2
my_demo-objs := my_demodrv.o

obj-m := mydemo.o
all:
	$(MAKE) -C $(BASEINCLUDE) M=$(PWD) modules;
clean:
	$(MAKE) -C $(BASEINCLUDE) SUBDIRS=$(PWD) clean;
	rm -f *ko;
