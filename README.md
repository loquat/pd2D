# pd2D 0.1 (pre-alpha)

## pd2D is a high-performance, zero-dependency 2D graphics library for classic VB 

## Project status

pd2D is in alpha status.  It is not feature-complete, but its GDI+ backend already supports a large variety of rendering tasks.

The bulk of the library's API *should* be stable, but small changes are possible between now and a 1.0 release.  The library's rendering code is (mostly) stable and (mostly) leak-free.  

Feedback is very welcome, particularly regarding the library's design.  There's plenty of time to modify things before a 1.0 release.  (A timeline for said 1.0 release is still nebulous... but it won't be until the end of summer at the earliest, so I can guarantee a decent amount of testing.)

## Other things to know:

### pd2D is 100% open-source

pd2D is derived from the open-source PhotoDemon photo editor (https://github.com/tannerhelland/PhotoDemon).  Like its parent project, pd2D is available under a liberal BSD license.  This license allows you to use the library in any project, commercial or otherwise.  (Please see the LICENSE.MD file for specific details, including disclaimer of warranty.)

You are also free to fork this library and/or make your own modifications.  (And of course, I am very happy to look at pull requests - so send over your bug fixes and new features ASAP!)

### pd2D has no external dependencies

The library's default backend leans on standard libraries available all the way back to Windows XP.  Windows XP through the latest Windows 10 builds are considered "fully supported."

### pd2D is designed with multiple backends in mind

The default pd2D build uses a mixture of GDI, GDI+, and custom code, but it can easily be extended to support other backends.  For example, you could wrap pd2D's API around a 2D library like Cairo with little effort.  Suggestions for alternate backends (or even better, pull requests!) are always welcome.

### pd2D does not require you to be a graphics expert

Unlike a bare type library, pd2D manages things like memory allocations and handle disposal for you.  If you know how to use VB6 classes, you know everything you need to use pd2D.

### pd2D is fast and lightweight

Wherever possible, pd2D leans on hardware-accelerated rendering.  Performance is best under Windows 10, but some measure of hardware acceleration is available all the way back to Windows XP.

### How can I get involved? 
pd2D is maintained by a single individual with a family to support.  The software is provided free-of-charge under a permissive open-source license, and no fees will ever be charged for its use.

That said, donations go a long way toward supporting its development.  If you would like to donate and support development, you can donate through pd2D's parent project website:

http://photodemon.org/donate/

If you can't contribute monetarily, here are some other ways to help:
* Let me know if you find any bugs. Issues can be submitted via pd2D's official bug tracker: https://github.com/tannerhelland/pd2D/issues
* Pull requests (for bug-fixes, new features, new backends, documentation - anything!) are always welcome.
* Do you wish pd2D behaved differently?  Do you want it to offer a particular feature?  Let me know!  Suggestions and feedback are always welcome, and they can be submitted through the same bug tracker: https://github.com/tannerhelland/pd2D/issues

### How do I use pd2D?

This repository is divided into two parts: the bare pd2D source (available in the /pd2D folder), and various sample projects (available in the /samples folder).  Start with the sample project that interests you most.  They are all thoroughly commented.

I am still fleshing out the sample project collection, so if there's something in particular you'd like to see, please let me know.