# tools

Notes By FML927

### Host: 
ubuntu 12.04-32bit

### compile for: 
Raspberry Pi 2

### used Tools version: 
fold "arm-bcm2708/arm-bcm2708hardfp-linux-gnueabi"
version SHA:f5642106425d430e1f82ee064121a5fd0e05a386
gcc veersion 4.8.3

### config:
download and config it cross compile for app.

config:(<http://blog.csdn.net/embbnux/article/details/17360315>)

'''
export PATH=$PATH:/......../arm-bcm2708hardfp-linux-gnueabi/bin
export CFLAGS="-O2 -pipe -mcpu=arm1176jzf-s -mfpu=vfp -mfloat-abi=hard -w" 
'''

can add the two line to "gedit ~/.bashrc"

###usage example: (tool name is a file name in fold ./arm-bcm2708/arm-bcm2708hardfp-linux-gnueabi/bin)
arm-linux-bnueabihf-gcc -o hello helllo.c
