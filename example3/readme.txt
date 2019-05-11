1,编译: arm-linux-gnueabi-gcc test.c -o test --static
2,运行: insmod mydemo.ko,使用cat /proc/devices查看设备信息
然后使用mknod /dev/demo_drv c 252 0在/dev目录下生成对应的节点
