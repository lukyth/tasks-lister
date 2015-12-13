# Tasks Lister
> A kernel module that lists all current tasks in a Linux system

This is a project for my Operating System class, Computer Engineering, Kasetsart University.

The assignments are comming from a book "Operating System Concepts, 9th Edition", Chapter 3 - Process Concept, Project 2 - Linux Kernel Module for Listing Tasks.

### Part I Assignment  
Design a kernel module that iterates through all tasks in the system using the `for_each_process()` macro. Make the contents appear in the kernel log buffer.

### Part II Assignment
The same as Part I but use DFS tree instead.

## Installation
```
$ git clone https://github.com/lukyth/tasks-lister.git
$ cd tasks-lister/
```

## How to use
```
$ cd src/[linear|dfs]
$ make                                  # Make module
$ insmod tasks_lister_[linear|dfs].ko   # Install module
$ dmesg                                 # Show message
$ rmmod tasks_lister_[linear|dfs]       # Remove module
$ dmesg                                 # Show message
$ dmesg -C                              # Clear message
```
