---
layout: default
title: Download
is_main: true
---

The project can be splitted in two different branches.
The first branch is the version released during 2014, which is quite stable and will not get improvements (except bug fixes, if any).
The second branch is the current developement version, which began in 2015. It have important structural changes, and some API changes, comparing to the 2014, so that it is not hosted in the same repository.

# Development version (after 2015)

The [current version](https://github.com/AversivePlusPlus/AversivePlusPlus) has no release yet.
You can check the [wiki](https://github.com/AversivePlusPlus/AversivePlusPlus/wiki) 
to see installation tutorials.

Even without release, we manage to make the master branch always buildable.
You can check if the current master version is buildable with this label :

![build?](https://travis-ci.org/AversivePlusPlus/AversivePlusPlus.svg?branch=master)

It is automatically generated for each push action.

# Old stable version (2014)

These [stables versions](https://github.com/astralien3000/aversive--) were released in 2014. 
They support ATMega2560 and ATMega128 microcontollers, with only a few specific devices supported.
You can also use it with the [SASIAE simulator](https://github.com/astralien3000/tinySASIAE), 
that was developed by the same team as the library.

## v14.11 (beta)

This version is intended to be used with the simulator, and every known bugs have been fixed (if you find one, please, contact us ;) ! )
It is used for teaching basics of 2 wheeled robot control.

 - [Aversive++ v14.11](https://github.com/astralien3000/aversive--/archive/v14.11b.tar.gz)
 - [tinySASIAE v14.11](https://github.com/astralien3000/tinySASIAE/archive/v14.11.tar.gz)
 
## v14.06 (alpha)
 
This version was embedded on a real robot using an atmega128.
 
 - [Aversive++ v14.06](https://github.com/astralien3000/aversive--/archive/v14.06.tar.gz)
 - [tinySASIAE v14.06](https://github.com/astralien3000/tinySASIAE/archive/v14.06.tar.gz)
 
## An example code

You can also download the example project using Aversive++ v14.06 and tinySASIAE v14.06, that simulates a two-wheeled robot.
The example is tested for linux. The dependencies are g++ (> 4.7), and Qt5.
(Be careful, the include path for qt5 used in the Makefile is different for some distributions. You may have to change it)

 - [Teaching material](https://drive.google.com/file/d/0B9V_NolZXjZ-SGczc0o0RDdzeXc/view?usp=sharing)

To compile and run the project, just do :

 - `cd tinySASIAE/robot`
 - `./deploy.sh`

A window showing a moving robot should appear.

If you use Ubuntu or an other debian-like distribution,
the compilation may fail because of the include path of Qt5. You should change this line in the Makefile :

 - `SASIAE_INCLUDE= $(GEN_INCLUDE)/sasiae -I/usr/include/qt5 -I/usr/include/qt5/QtCore`

And replace it by :

 - `SASIAE_INCLUDE= $(GEN_INCLUDE)/sasiae -I/usr/include/x86_64-linux-gnu/qt5 -I/usr/include/x86_64-linux-gnu/qt5/QtCore`
