UPDATE: The scantailor-enhanced 20120727 package has been added. Please report any bugs to me.

(Version 0.9.11.1 might be more stable but has fewer features)

Scan tailor requires the QT runtime package which takes forever to compile and install on any system.  This project aims to distribute binaries in an effort to increase the usage of opensource on the Mac platform.  The current packages are built with the supplied prebuilt QT4 package. The App is in Aqua, not X11, so it looks rather nice.

Version 0.9.11.1 is an Intel (32bit) binary built on my snow-leopard machine. It should run on 10.4+

Enhanced 20120727 is an x64 binary built for Mountain Lion, It should run on 10.7+


There are two sets of files currently available:
The first (withoutCLI) does not include the command line interface binary and only includes the QT-based GUI.

The second (withCLI) is the same app, though also includes the command line interface binary. It exists at Scantailor.app/Contents/MacOS/scantailor-cli
It has relative links within the app, so do NOT take it out of the package. If you would like to be able to access it more easily, create a symbolic link from within your $PATH. (something along the lines of

`$ sudo ln -s /path_to_the_app/ScanTailor.app/Contents/MacOS/scantailor-cli /usr/bin/scantailor-cli`


I have one note for an issue you might encounter: if you have an image (say, a PNG) with the file extension of another type (say .JPG), Mac os x will work with it, but scantailor will be very confused and will refuse to load the image. If you have that problem, check to ensure your extensions are correct.