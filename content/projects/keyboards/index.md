+++
title = "QMK and RISC-V"
date = 2023-10-21

[taxonomies]
categories = ["hardware"]

[extra]
featured_image = "image.jpg"
+++

Contributing RISC-V support to the ChibiOS RTOS and allowing for effecient multithreaded LVGL rendering in QMK. 

<!-- more -->

The QMK keyboard software is a powerful open-source firmware that allows users to fully customize the functionality of their keyboards. QMK is based on the ChibiOS RTOS, a real-time operating system that is designed for embedded systems.

I contributed to the ChibiOS RTOS by adding support for the RISC-V architecture. RISC-V is a free and open-source instruction set architecture (ISA) that is gaining popularity in the embedded systems market. My work on ChibiOS made it possible to use QMK on RISC-V based keyboards.

After adding RISC-V support to ChibiOS, I designed an ergonomic RISC-V based keyboard. This keyboard was designed to be comfortable to use for extended periods of time. It features a split design, which allows the user to position the keyboard halves in a more natural position. The keyboard also features a number of other ergonomic features, such as tenting and columnar staggering.

My next project is to develop a keyboard that features a memory-LCD display. Memory-LCDs are a type of display that can retain an image without the need for power. This makes them ideal for use in keyboards, as they can be used to display information such as keymaps and macros.

In addition to adding memory-LCD support, I am also designing SPI-driven matrix hardware for the keyboard. SPI is a serial communication protocol that is commonly used in embedded systems. By using SPI to drive the matrix, I can reduce the number of pins that are required to connect the keyboard to the microcontroller.

I am excited to continue working on the development of custom keyboards. I believe that custom keyboards have the potential to be more comfortable, more functional, and more aesthetically pleasing than off-the-shelf keyboards.

I have attached an image above of the schematics for the upcoming keyboard design.
