## Intro to Embedded Linux

### Four Elements of Embedded Linux

1. Toolchain

    The compiler and other tools that are needed to create code for the target device. *Everything depends on the toolchain*


1. Bootloader

    The program that initializes the board and loads the Linux Kernel


1. Kernel

    This is the heart of the system that manages resources and interfaces with the hardware layer of the board

1. Root File System

    Contains the libraries and programs that run once the system has completed its initialization. Source code is a part of the root file system.
