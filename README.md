# "One Formula That Demystifies 3D Graphics"

The Source Code from this YouTube Video:

[![thumbnail](./imgs/thumbnail.png)](https://www.youtube.com/watch?v=qjWkNZ0SXfo)

## Quick Start

.................

## Port it to RPI4

```console
$ git clone https://github.com/sidd-kishan/formula
$ cd formula
$ git submodule update --init
$ cp -r 44-3dCPURender/ circle/sample
$ cd circle
$ ./configure -r 4 -p "aarch64-none-elf-" --multicore --qemu -f
$ ./makeall
$ cd sample/44-3dCPURender/
$ qemu-system-aarch64 -machine raspi4b -cpu cortex-a72 -m 2G -kernel kernel8-rpi4.img -serial stdio
$ 
```



https://github.com/user-attachments/assets/b7a24c7d-04c7-4015-8664-782095279b02

*Disclaimer: Assistance from Cursor was also used in this port 

The model is provided by [https://github.com/Max-Kawula/penger-obj](https://github.com/Max-Kawula/penger-obj)

[![penger-obj](./imgs/penger-obj.png)](https://github.com/Max-Kawula/penger-obj)


