## Hello World of Poky

1. Make a source folder

1. Change directory to it

1. git clone the repo
            
            git clone git://git.yoctoproject.org/poky


1. Once done, it will have many folders some of them are

    - BitBake - schedular of the poky
    - meta-poky - poky related meta-data
    - meta-yocto-bsp - BSP's supported by yocto project for boards like BeagleBone, Edge router
    - meta-OE core related meta-data

1. Checkout the *ZEUS* release or branch

1. Prepare the build environment
    
    - Running the file oe-init-built-env will setup all the build environment/path and setup for running yocto project in the PC

    - If you run bitbake command it will through an error that is command is not found

    - Beacuse *$PATH* does not has been set

    - run source oe-init-built-env ../../build

    - Once the setup is done successfully, if you give *$PATH* it lists the path of yocto related contents also.

    - Now run, bitbake -h command.

    - Previously we would have been in the poky folder, now we will be in build folder

    - Conf files will be created; Use the command tree config to list them.

    - To Create files run 
            
            bitbake core-image-minimal
    
    - Bitbake does the following,

        - It parses the metadatas
        - Schedules the tasks
        - Declare the configuration
        - Initialize the tasks
        - Executes the tasks

    - Common linux commands

            nproc => lists no.of cores
            free -m => lists RAM space