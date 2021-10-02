# AnonymousSubmission185

Introduction of the tested applications and benchmark.

### PinLock

This application is an unofficial smart lock running on the STM32F4-Discovery board. When it first starts up, the application prompts the user to enter the correct pin code. Next it receives the pin code from the serial port. The application then uses the functions of mbedtls library to compute the hash of the received pin code.
The result is compared with a stored value. If the pin is correct, an LED will be turned on to indicate the unlock state. Otherwise, the application will continue to ask a new user input.

Code: https://github.com/embedded-sec/ACES/tree/master/test_apps/pinlock

### Camera

This application uses the camera on the STM32469I-EVAL board to take a photo after the user press the button. The photo is stored as a BMP file at a USB disk.

Code: https://github.com/STMicroelectronics/STM32CubeF4/tree/master/Projects/STM32469I_EVAL/Applications/Camera/Camera_To_USBDisk

### Animation

This application demonstrates a moving butterfly against the background of the ST logo on the screen.

Code: https://github.com/STMicroelectronics/STM32CubeF4/tree/master/Projects/STM32469I_EVAL/Applications/Display/LCD_AnimatedPictureFromSDCard

### LCD-uSD

LCD-uSD presents the pictures stored in the SD card with fade-in and fade-out effects.

Code:  https://github.com/STMicroelectronics/STM32CubeF4/tree/master/Projects/STM32469I_EVAL/Applications/Display/LCD_PicturesFromSDCard

### Fatfs-uSD

Fatfs-uSD implements a FAT file system on a micro SD card. It writes some fixed contents to a newly created file in the file system.
After that, it reads the file and checks whether the content is correct.

Code: https://github.com/STMicroelectronics/STM32CubeF4/tree/master/Projects/STM32469I_EVAL/Applications/FatFs/FatFs_USBDisk

### TCP-Echo

This application runs a TCP echo server on the board. The server is developed based on lwIP~\cite{lwIP}, which is a lightweight implementation of TCP/IP protocol.

Code: https://github.com/STMicroelectronics/STM32CubeF4/tree/master/Projects/STM32469I_EVAL/Applications/LwIP/LwIP_TCP_Echo_Server

### CoreMark

EEMBC’s CoreMark is a benchmark that measures the performance of microcontrollers (MCUs) and central processing units (CPUs) used in embedded systems. Coremark contains implementations of the following algorithms: list processing (find and sort), matrix manipulation (common matrix operations), state machine (determine if an input stream contains valid numbers), and CRC (cyclic redundancy check). It is designed to run on devices from 8-bit microcontrollers to 64-bit microprocessors.

Code: https://www.eembc.org/coremark/
