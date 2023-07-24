## QEMU

1. Quick Emulator is a free/open source tool that runs hardware virutualization

1. This tool allows testing and development without any real hardware

1. Currently QEMU supports 

    1. ARM
    1. MIPS64
    1. x86
    1. MIPS
    1. PowerPC
    1. X86_64

1. Poky provide scripts called "run qemu" which allows us to run yocto generated images using QEMU

1. *runqemu qemux86_64 core_image_minimal* - QEMU opens the bootlog of the image

1. runqmeu < machine > < Zimage > < file system >

1. < machine > => Machine architecture to use

    - qemuarm
    - qemumips
    - qemuppc
    - qemux86
    - qemux86_64

1. < Zimage > => Path to the kernel

1. < File System > => Path to the ext image

1. The configuration files of QEMU can be changed on ./build/conf/local.conf

1. Configuration like

    - MACHINE
    - Enable/Disable tools like KVM ( Kernel based Virtual Machine )
    - If arguments are not specified then the default configuration are used like QEMUARM for machine and EXT4 for file system

1. Using QEMU, we can get the CPU info using *get CPU info* and shutdown the device using *shutdown*
