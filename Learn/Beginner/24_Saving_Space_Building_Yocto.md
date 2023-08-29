## Saving disk space while building yocto

- Yocto builds system can take a lot of disk space during build. But bitbake provides to preserve disk space

- We can command bitbake to delete all the source code, build folder, build files after building a particular recipe by adding the following line in local.conf file
*INHERIT += "rm_work"*

- Disadvantage: Difficult to debug which build fails of any recipe. For example: if you want to exclude bitbake deleting source code of a particular package, you can add it in 
*RM_WORK_EXCLUDE += "recipe-name"*

- example: *RM_WORK_EXCLUDE += "core-image-minimal"*