+++
title = "Asahi Linux"
date = 2023-10-21

[taxonomies]
categories = ["software"]

[extra]
repo_path = "AsahiLinux/linux"
featured_image = "image.jpg"
+++

Helping Reverse engineering Apple Silicon devices and upstream drivers into the Linux Kernel

<!-- more -->

The Asahi Linux project is a community-driven effort to bring Linux to Apple Silicon Macs. The project has made significant progress in reverse engineering the hardware and software of apple's proprietary hardware, and has successfully booted Linux on a variety of models.

One of the key challenges in porting Linux to Apple Silicon is the lack of documentation for the hardware. As the hardware is meant to only function with MacOS, documentation ranges from sparse to nonexistent, and so *everything* needs to be reverse engineered. 

My contributions to the Asahi Linux project have focused on reverse engineering the D3DMetal API on macOS, integrating it with the M1N1 supervisor for integrated debugging, and reverse-engineering the extensions apple has made to the ARM specification, specifically those related to Matrix Coprocessing. I have then implemented support for these extensions and architectures under Linux and several open source tools (including numpy). 

I am proud to be a part of the Asahi Linux project. The project is a testament to the power of open source software. By working together, the Asahi Linux team has been able to achieve what would have been impossible for any individual. I am excited to see what the future holds for the Asahi Linux project, and I am confident that the project will continue to make significant progress in bringing Linux to Apple Silicon Macs.

Further information: https://asahilinux.org