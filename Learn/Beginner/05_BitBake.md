## Bitbake

- Bitbake is a core component of the yocto project

- It is basically performs the same functionality of *make*

- It's a task schedular that parses python and shell mixed code

- The code parsed generates and runs tasks, which are basically set of steps ordered according to the code's dependencies

- It reads recipes and follows them by fetching packages, building them and compiling them into bootable images.

- It manages all tasks and make track of complition in reasonable time by maxing the result
