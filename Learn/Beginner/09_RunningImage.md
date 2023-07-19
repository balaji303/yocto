## Running Image

1. We can also run QEMU without graphics or bootup screen

1. *runqemu qemuarm nographic* or *runqemu core-minimal nographics*

1. Without the UI everylog will run in the console itself

1. Comments like *ls* and *cd* are working but not *lsusb* or *mc* or *bc*

1. Comments like lsusb is not working in the yocto image that we just generated and ran. 

1. This is because the generated image has no recipe called usbutils

1. USButils is the recipe that controls USB devices

1. To Add a particular recipe use 
*IMAGE_INSTALL += "recipe_name"* or *IMAGE_INSTALL_append = " usbutils"*

1. For LUSB use IMAGE_INSTALL += "usbutils"

1. Add the above line in config file in *build/conf/local.conf*

1. Do bitbake and generate the image again.

