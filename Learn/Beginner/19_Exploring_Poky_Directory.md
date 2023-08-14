## Exploring Poky directory


### BitBake

- Holds all python scripts used by the bitbake command *bitbake/bin* is placed in to the path environmental variables so bitbake can be found

### Meta

- Contains the OE-Core metadata

### Meta-Poky

- Holds the configuration for the poky reference distribution local.conf.sample, bblayer.conf.sample are present here

### Meta-Skeleton

- Contains template recipes for BSP and Kernel development

### Meta-Yocto-BSP

- Maintains several BSP such as Beagble Bone, Edge Router and geenric versions of both 32 & 64 bit machines

### Scripts 

- Contains several scripts that are used to set up the environment, development tools and tools to flash teh generated images on the target

### License

- The license details of the poky

### Documentation

- All documentation source for the Yocto Project documentation. Can also be used to generate PDFs