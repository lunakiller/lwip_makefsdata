## Instructions
To generate *fsdata.c* file for lwIP:

1) Use the Perl script makefsdata
2) Compile *makefsdata.c* console program
    - Copy *lwipopts.h* (for STM32 projects, it is in folder *LWIP/Target*)
    - Comment `#include "main.h"` (~line 25) 
    - run
    `gcc makefsdata.c -I. -I../../../include/ -I../../../../system/ -o htmlgen` and pray that it works...
    - if you need more data types (eg. svg), add: `-D'HTTPD_ADDITIONAL_CONTENT_TYPES={"svg", HTTP_HDR_SVG}'`
        - refer to *httpd_structs.h*

