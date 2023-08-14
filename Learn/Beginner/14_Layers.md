## LAYERS

1. Layers are a collection of related receipes or a recipe containers

1. poky has the following layers

    - Meta
    - Meta-poky
    - Meta-SelfTest
    - Meta-Skeleton
    - Meta-Yocto-BSP

1. Layers provide a mechanisms to isolate meta-data according to functionality for instance BSPs, distribution, configuration, etc.

1. Using this concept we can add, remove, reuse different modules like BSP, GUI, Distro Configuration, Middleware or app.

1. *build/conf/bblayer.conf* files has variables used by the poky during build. *bblayer.conf* us created by the bitbake when *bblayer.conf* is not present.
