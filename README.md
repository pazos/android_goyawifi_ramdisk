[RAMDISK]

Stock ramdisk from T110XXUANI7 boot.img

	Changelog:
		- Disable marvell powerdaemon to be able to modify current governor & IO scheduler

[KERNEL]

From https://github.com/pazos/android_kernel_samsung_goyawifi.git

[SCRIPT]

mkboot is a simple script to automate the build.

	This script will download the kernel sources for SM-T11x into linux/ 
	and build a new boot.img with those kernel sources and current ramdisk:

	./mklinux boot-img	--> Build a new boot.img based on ramdisk & kernel binaries or sources"

	./mklinux build		--> Forces a new kernel build and update kernel & module binaries"

	./mklinux menuconfig	--> Edit kernel configuration"

	./mklinux mrproper	--> Clean kernel tree"

	The script needs to be called from the same directory 
	(ie: downloads/goya/mklinux boot-img will not work)
