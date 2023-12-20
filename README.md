**This is just a placeholder repo with no actual weenix source code in order to adhere to Brown University's Academic Code. If you would like to view the code please send me an email at naafiyan@gmail.com**

A UNIX-based Operating Systems kernel, built over the course of a semester in Brown University's CSCI 1690 (Operating Systems). You can find the weenix handout [here](https://github.com/brown-cs1690/handout/wiki). 

Each of the following projects built an essential component of the Weenix OS:
1) Procs: Implementation of threads, processes and synchronization primitives
2) Drivers: device drivers for terminals, disks, and the memory devices `/dev/zero` and `/dev/null`
3) VFS (Virtual File System): Polymorphic interface in C to abstract away interactions betwen the OS kernel and file systems such as S5FS
4) S5FS (System V File System): Implementation of file system based on the original Unix file system
5) VM (Virtual Memory): Allowing for the OS kernel to manage user address spaces, run user-level code and servicing system calls. Implementation consists of:
    - Virtual Memory Maps
    - Page Fault Handler
    - Anonymous objects to handle allocation of pages for non-persistent data
    - Shadow objects to allow for the `fork()` system call
        - Shadow collapse to cleanup shadow chains
    - Trapping to OS kernel for system calls
