+++
title = "WP43"
date = 2023-10-21

[taxonomies]
categories = ["calculators"]

[extra]
featured_image = "image.jpg"
+++

A modern take on HP RPN calculators of old, utilizing the RPN format and the spirit of the 32S, 32Sii, & 42S

<!-- more -->

# What is RPN?

I was always obessed with calculators: handheld primitive computers to carry out primitive calculations. The issue is modern calculators follow an algebraic system (often referred to as textbook notation), what you see is what you get. While in theory this sounds excellent as students can directly type in equations from their textbook, in actuallity it works against our thought process

HP solved this problem decades ago in the form of RPN: reverse polish notation. Originally drafted to overcome the memory and processing limitations of the time and heavily taking advantage of a `stack`, the "language" grew favored by many. 

The main benefit of such a formal logic system is it allowed mathematical expressions to be specified without parenthesis by placing the operators before (prefix notation) or after (postfix notation) the operands. 

# Why RPN?

In that sense, RPN/RPL operate like lisp, inwards to out. Your brain thinks this way. Any actual problem is solved this way. You want to know the results of intermediatary steps and store them. Make one problem? You should be able to build on it, return to the previous step, etc. Algebraic calculators don't work this way 

Same with solving equations or writing programs. RPN makes you write out the RHS of an equation in calculator operations, the same steps you'd take if you were trying to solve it on paper yourself.

In the years that followed, computer scientists realized that RPN or postfix notation was very efficient for computer math. As a postfix expression is scanned from left to right, operands are simply placed into a last-in, first-out (LIFO) stack and operators may be immediately applied to the operands at the bottom of the stack. By contrast, expressions with parentheses and precedence (infix notation) require that operators be delayed until some later point. Thus, the compilers on most modern computers converted statements to RPN for execution. (In fact, some computer manufacturers designed their computers around postfix notation.)

At the time that the HP-35 was introduced, other pocket calculators typically used a partial algebraic model. That meant they could evaluate trivial expressions like 4+5 but couldn't handle anything that involved parentheses or algebraic precedence. The technology of the time didn't allow for full algebraic compilers in pocket calculators.

RPN allowed HP to produce a pocket calculator that could evaluate arbitrary expressions using the available technology. For many, learning a new style of entry was a small price to pay to be able to evaluate arbitrary expressions on a calculator. Once the technology to produce algebraic compilers could fit into a pocket calculator, most RPN users had decided that RPN was more efficient and consistent for the user as well as for the calculator. Also, because subexpressions are evaluated as they are entered, entry errors are more obvious with RPN. On an algebraic calculator, omitting an opening parenthesis, may not lead to a calculation error until much later when an entire subexpression is evaluated.

Sadly, as technology evolved, calculators became cheaper, and as TI essentially monopolized the mathematics education space, HP was force to give up RPN and adapt an algebraic-adjacent system. They itereated on this with the HP48 and HP50 series, allowing for arbitrary execution of algebraic subsystem (even going as far to include a symbolic system), but ultimately TI's stronghold on the market was too strong and HP sold off their calculator business

# Introducing: C43

Now for the C43 project itself. Even though RPN was no longer mainstream, there are many developers, electronic engineers, and mathematicians who liked the simplified and intuitive workflow of an RPN calculator. However, as HP had stopped producing the HP42 and HP32SII series (the last and most beloved proucts of the RPN era), supply was drying up and the few mint editions left were going for hundreds of dollars. 

Enter Free42 and Swissmicros: together partnering with open source software and hardware, they created a modern implementation of the HP42s through emulation and extensions, most notably an 8-level stack reducing the need for memory tricks. However, the question was raised: instead of emulating an outdated HP42, what was possible if we were set with free reign?

At the same time, I was working on Calc-RS: a rust implementation of the RPN subsystem complete with an abritirarily large RPN stack, acurate decimal arithmatic, exact rationals, unit conversions, all rendering under a GTK frontend. Several other developers were working on similar projects in forth, lisp, and whatnot

Swissmicros proposed a project to all of these devs, me included: what if everyone got together to implement a modern take on an HP RPN calculator on modern hardware? And so the WP43 project was born.

Each of us were sent development versions of a DM42 with modified key-layout running a modified bootloader, and were left with free reign on the userspace software. 

The end result is shown above: a modern RPN calculator with 8-level stack, 128-bit decimal precisions for financial calculations, statistics, probability, and various other solvers (along with the algebraic solver of the 32SII), proper mixed types (which had never been implemented in an RPN calculator until that point). 

Each key has two different submenus, each with 3 stacks of functions and dedicated keys, all running an STM32 arm processor against a Sharp Memory LCD, offering similar power benefits to an E-INK display, running over 6 months on a coin-cell!

And most importantly, it retains all of the RPN programability of its ancestors

Sadly, in the end the project was deemed to be unprofitable and so the official hardware project was cancelled, and the software lives on with community support renamed to "Classic47". 

Regardless of its fate, I'm glad to have worked on such a project with experienced professionals around the world, and I am evermore grateful to own a functional piece of calculator history. 

You can find further details of the project under its new home at https://47calc.com. 