# Exploring Build Folder

- When we run source oe-init-build-env file it will create "build" folder in that dir

- The build folder has /build/conf which has 2 important files
    - local.conf
    - bblayer.conf

### local.conf

1. Configures every aspect of the build system with local user settings
1. MACHINE = The machine to which the target is build for 
1. DL_DIR = where to place downloads. During the first build the system will download many different source code. The default place to store these is the download dir under TOP_DIR which is build DIR
1. TEMP_DIR = The place where build output and also where bulk of the building work should be done and placed
1. BB_NUMBER_THREADS = Determines the number of tasks that bitbake will perform in parallel 
```$bitbake -e core-image-minimal | grep ^BB_NUMBER_THREADS=```
1. PARALLEL_MAKE = corresponds to the "-j make" options specifies the no.of process that GNU make can run in parallel on a compilation task
```$bitbake -e core-image-minimal | grep ^PARALLEL_MAKE=```