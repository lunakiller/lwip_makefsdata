## Instructions
To generate fsdata.c file for lwIP:

1) Use the Perl script makefsdata
2) Compile makefsdata.c console program
    - Copy lwipopts.h from STM32 project, folder LWIP/Target
    - Comment `#include "main.h"` (~line 25) 
    - run
    `gcc makefsdata.c -I. -I../../../include/ -I../../../../system/ -o htmlgen` and pray that it works...
