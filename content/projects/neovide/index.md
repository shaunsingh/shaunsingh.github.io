+++
title = "Neovide: Neovim GUI in Rust"
date = 2023-10-21

[taxonomies]
categories = ["editing"]

[extra]
repo_path = "neovide/neovide"
featured_image = "image.jpg"
+++

Porting the Neovide GUI to OpenGL and MacOS, and maintaining underlying rust libraries

<!-- more -->

Neovide is a popular graphical user interface (GUI) for the Neovim text editor. It is written in Rust and uses the Vulkan graphics API. WGPu is a Rust library that provides a safe and idiomatic wrapper around the WebGPU API.

I helped implement the OpenGL renderer for Neovide using the tried and true Skia library. This was a challenging task, as it required me to learn about the OpenGL API and how to use it to render text and other graphical elements, whereas I had largely focused on Terminal applications beforehand. I also had to ensure that the renderer was performant and did not introduce any regressions.

In addition to working on the OpenGL renderer, I also helped add support for macOS to Neovide. This involved porting the codebase to macOS and ensuring that it compiled and ran correctly. I also had to make some changes to the user interface to make it more macOS-friendly.

I also added multithreading support to Neovide. This allows the GUI to perform tasks such as syntax highlighting and code completion in parallel. This can significantly improve the performance of the GUI, especially on large files.

In addition to working on Neovide itself, I also maintain the underlying Rust libraries that Neovide depends on. This includes the wgpu library, as well as the neovide-renderer library.

Maintaining these libraries is a challenging task, as it requires me to stay up-to-date on the latest changes to the Rust language and the underlying graphics APIs. I also have to ensure that the libraries are compatible with the latest versions of Neovide.

I am proud to be a contributor to the Neovide project. It is a great example of how open-source software can be used to create high-quality software. My contributions to Neovide have helped to make it a more powerful and user-friendly text editor.

My work on Neovide led to an internship at Zed, a company that is developing a new kind of text editor. At Zed, I am working on a new GUI for the editor that is based on the Neovide codebase. I am excited to be able to continue working on Neovide and to help make it the best text editor possible.

You can find further information at https://neovide.dev