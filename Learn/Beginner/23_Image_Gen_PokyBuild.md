## Image generation by the poky build

- The build process writes images out of the build directory inside the tmp/deploy/images/machines folder

### Kernel  folder

A Kernel binary files the KERNEL_IMAGE_TYPE variable determines the naming scheme for the kernel image file

```$bitbake -e core-image-minimal | grep  ^KERNEL_IMAGETYPE=``` 

ex: "bzimage"

This is present in /tmp/deploy/image/qemux86_64

### root-filesystem-image

Root file system for the target device (eg. *.ext3 or *.bz2 file)

The IMAGE_FS_TYPES variable determines the root file system image type

```$bitbake -e core-image-minimal | grep  ^IMAGE_FSTYPES=``` 

### Kernel- Modules

Torballs that contains all the modules build for the kernel

### Bootloaders

If applicable to the target machine, bootloaders supporting the image.

### Symlinks

Symbolic link pointing to the most recently file for each machine these might be useful for external scripts that need to obtain latest version of each file
