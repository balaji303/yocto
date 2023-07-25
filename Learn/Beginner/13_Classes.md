## Classes

1. Class files are used to abstract common functionality and share it among multiple recipe files

1. To use a class file you simply make sure the recipe inherits the class

Example:

- cmake.bbclass - Handles cmake is recipes
- kernel.bbclass - Handles building kernels. Contains code to build kernel tree.
- module.bbclass - Provides support for building out-of-tree linux kernel modules.

3. Class are present in /poky/meta/classes