# AMJ66
AMJ66 Keyboard tmk firmware

## Compiling on Linux
Install the needed dependencies

    sudo apt-get install -y git unzip build-essential
    sudo apt-get install -y make gcc-avr avr-libc binutils-avr dfu-programmer
    sudo apt-get install -y binutils-arm-none-eabi gcc-arm-none-eabi libnewlib-arm-none-eabi libstdc++-arm-none-eabi-newlib dfu-util

Clone the repository, including submodules (requires Git  1.9

    git clone --recursive https://github.com/FSund/AMJ66.git

Compile

    cd AMJ66/src
    make clean
    make all

You can now burn the hex `AMJFC660M_lufa.hex` to the keyboard using your favourite tool.

## Bootloader
Hold Shift+B while inserting the USB cable to enter bootloader/programming mode.
