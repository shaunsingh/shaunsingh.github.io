+++
title = "Emacs"
date = 2023-10-21

[taxonomies]
categories = ["editing"]

[extra]
repo_path = "emacs-mirror/emacs"
featured_image = "image.jpg"
+++

Implementing support for apple silicon, XWIDGETS and webkit-based browsing, and SQLITE support in modern emacs. 

<!-- more -->

Emacs is a self-documenting text editor that has been in development for over 40 years. It is known for its powerful customization features, which allow users to tailor the editor to their own needs. Emacs is also known for its Lisp-based extension language, Emacs Lisp, which allows users to write code that can be used to extend the functionality of the editor.

In many ways, Emacs can be considered a modern-day Lisp machine. Lisp machines were computers that were designed to run Lisp code natively. Emacs is not a Lisp machine in the traditional sense, but it does provide a Lisp-based environment that can be used to develop and run Lisp code.

The use of Lisp in Emacs has a number of benefits. First, Lisp is a very expressive language that is well-suited for writing code that is both powerful and elegant. Second, Lisp is a very dynamic language, which means that code can be modified and evaluated at runtime. This makes it possible to write code that is highly interactive and responsive.

Emacs's introspectability is another feature that makes it a powerful tool for development. Introspection is the ability of a program to examine its own state and behavior. Emacs provides a number of features that allow users to inspect the state of the editor and the code that is running within it. This makes it possible to debug code more effectively and to understand how the editor works.

Emacs's interactive coding experience is also a major benefit. Emacs allows users to evaluate code as they are typing it. This makes it possible to experiment with code quickly and easily. It also makes it possible to develop code in a more iterative manner, where small changes can be made and tested immediately.

I have made a number of contributions to Emacs. Some of my most notable contributions include:

- Xwidgets webkit browsing support: I helped implement support for the Xwidgets toolkit in Emacs, which allows users to embed web content within Emacs buffers. This makes it possible to use Emacs as a web browser (xwidgets-webkit).
- Cocoa Macport frontend: I helped port the Cocoa-based frontend for the MacPorts edition of emacs to modern instances of macOS. This includes fixing several bugs in GlibC preventing the compilation of EmacsMacport past LLVM9
- Support for ARM devices, Plan 9, and Apple Silicon: By allowing for a more modern compiler, I have helped port Emacs to a number of new platforms, including ARM devices, Plan 9, and Apple Silicon. This makes it possible to use Emacs on a wider range of hardware, and therefore a wider audience.
- SQLITE3 implementation in Emacs 29: I helped implement support for the SQLITE3 database engine in Emacs 29. This makes it possible to use Emacs to manage and query SQLITE3 databases.
- Org-roam V2 and org-roam-ui package: I am a maintainer of Org-roam V2, a major rewrite of the Org-roam package for Emacs. Org-roam is a tool for managing notes and tasks. Org-roam V2 is a complete rewrite of the original Org-roam package, and it includes a number of new features and improvements driven by the SQLITE integration detailed above. I am also a maintainer of the org-roam-ui package, which provides a graphical user interface for Org-roam through a react interface.

I am proud of the contributions that I have made to Emacs. I believe that Emacs is a powerful tool that can be used to do great things. I am committed to continuing to contribute to Emacs in the future.

The image above is an example rendering Org-Roam-UI notes with the now integrated WebKit browser, utilizing the Cocoa frontend for SVG and subpixel text rendering of the latex equations and text.