+++
title = "Maintaining Neovim"
date = 2023-10-21

[taxonomies]
categories = ["editing"]

[extra]
repo_path = "neovim/neovim"
featured_image = "image.jpg"
+++

Implementing first-party asyncronous LSP support into neovim, as well as improving on incremental semantic parsing techniques (tree-sitter) and Lisp + LuaJIT functional integration (fennel/LuaFUN). 

<!-- more -->

Neovim, a successor to the popular Vim text editor, is a highly customizable and extensible editor that has gained a devoted following among developers and power users. Its Lua integration allows users to extend the editor's functionality with Lua scripts, making it a versatile tool for a wide range of tasks.

I've had the pleasure of contributing to the Lua integration in Neovim in a number of ways. One of my early contributions was improving the forking and threading support in the LuaJIT library, which is used by Neovim to execute Lua scripts. This work made it possible for Lua scripts to safely create and manage child processes, which is essential for many types of plugins.

In addition to my work on the LuaJIT library, I've also written a number of Lua libraries for Neovim. One of my most popular libraries is luafun, a functional programming library for Lua. Luafun provides a number of features that are not available in standard Lua, such as higher-order functions, lazy evaluation, and monads.

I later ported luafun to Neovim as the plenary.nvim library. Plenary.nvim provides a powerful and expressive way to write Lua code for Neovim, and it has been used to implement a wide range of plugins.

In addition to my work on Lua, I've also contributed to Neovim's support for Tree-sitter, a parser generator for programming languages. Tree-sitter provides a powerful way to parse code, and it has been used to implement a number of syntax highlighting and code completion plugins for Neovim.

I've also worked on integrating Lisps into Neovim. This work has made it possible to use Lisp dialects such as Common Lisp and Fennel in Neovim plugins.

Finally, I've also contributed to a number of Neovim tooling projects, such as the nvim-lspconfig library for managing language servers and the nvim-cmp completion framework.

My contributions to Neovim have been a rewarding experience, and I'm proud to be a part of the Neovim community. I'm excited to see how Neovim continues to evolve in the future, and I'm committed to making further contributions to the project.
