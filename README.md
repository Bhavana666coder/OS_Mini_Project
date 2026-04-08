# Mini Container Runtime

This project implements a lightweight container runtime in C.

## Features
- Process creation using fork and exec
- IPC using pipes and UNIX sockets
- Multithreading using pthreads
- Bounded buffer logging system
- Separate log files for containers

## Run

gcc os.c -o engine -lpthread

sudo ./engine supervisor
sudo ./engine start 0 ./rootfs-alpha "echo Hello"
