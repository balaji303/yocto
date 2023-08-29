## Building Yocto Image for BBB

- Already yocto has the BSP for BBB
```source poky/oe-init-build-env build_bbb```

- Open build_bbb/local.conf file comment out the default selection of machine and select/uncomment
*MACHINE ?= "beaglebone-yocto"*

- Trigger Build: 
```$bitbake core-image-minimal``` use this inside build_bbb folder

- After the build is completed the image is ready at tmp/deploy/images/beaglebone

- Inside /source/poky/meta-yocto-bsp/conf/machine, There is beaglebone-yocto.conf

- What are the images contains:
    1. 1st level bootloader - MLO
    2. 2ed level bootloader - uboot,
    3. Kernel image,
    4. Device tree blobs,
    5. root-file system,
    6. Module archive



