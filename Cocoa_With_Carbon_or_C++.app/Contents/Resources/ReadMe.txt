Cocoa_With_Carbon_or_C++
========================

Cocoa_With_Carbon_or_C++ is sample code that shows how to call Carbon routines and C++ code from within an Objective-C/Objective-C++ Cocoa program.
The sample displays a window within which, depending upon the radio button selected, clicking the "Say Hello to the World" button will call functions
that use Objective-C, Carbon, or C++ respectively.

Calling Carbon routines is relatively easy, involving adding Carbon.framework to your project and including Carbon.h in your source code.
Because Objective-C is a superset of ANSI-C, calling Carbon C functions is not a problem.  One thing to note is that although it can be useful at
times to call non-GUI Carbon routines from Cocoa apps, functionality is more limited when attempting to include Carbon GUI in a Cocoa app.
This sample limits things to calling a modal alert panel.  Use of Carbon is now discouraged as it is not avaliable to 64-bit applications.

Calling C++ code from Objective-C code involves ending your file with .mm (instead of .m) so that the Objective-C++ compiler will be used.
This compiler can understand both C++ and Objective-C, although you still have to use Objective-C to call into the AppKit and Foundation classes.
In other words, the ObjC++ compiler lets you put C++ code directly in Objective-C methods, and vice versa, but it doesn't change which language you
must use when writing to the Cocoa APIs.

===========================================================================
BUILD REQUIREMENTS:

Xcode 3.2, Mac OS X 10.7 Lion or later

===========================================================================
RUNTIME REQUIREMENTS:

Mac OS X 10.7 Lion or later

===========================================================================
CHANGES FROM PREVIOUS VERSIONS:

Version 1.4
- Updated for Xcode 4.
Version 1.3
- Fixed compiler error, updated to use Xcode v2.4.1, Universal Binary, Carbon upgrade from .rsrc to .nib
Version 1.2
- Fixed a compile error on Project Builder 2.0.1/gcc3
Version 1.1
- Updated the sample to include use of the Objective-C++ compiler, on files that end in .mm
Version 1.0
- Initial version.

===========================================================================
Copyright (C) 2000-2011 Apple Inc. All rights reserved.