# Tasks Lister
A kernel module that lists all current tasks in a Linux system

## Installation
```
$ git clone https://github.com/lukyth/tasks-lister.git
$ cd tasks-lister/
```

## How to use
```
$ make                      # Make module
$ insmod <module_name>.ko   # Install module
$ dmesg                     # Show message
$ rmmod <module_name>       # Remove module
$ dmesg                     # Show message
$ dmesg -C                  # Clear message
```
