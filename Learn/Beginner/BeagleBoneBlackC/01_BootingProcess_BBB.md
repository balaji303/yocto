## Booting process in BBB

1. The AM335x is a complex piece of hardware, but has limited internal RAM (128kB)
1. Because of this limited amount of RAM, multiple bootloader stages are required
1. Since the size of bootloader will easing extent 128kB
1. These bootloader stages will unlock the full functionality of the device so that the complexity of the device are handled by the kernel
1. The stages of Bootloader are as follows

    1. ROM,
    1. SPL (Secondary Program Loader)
    1. U-Boot
    1. Linux kernel
    