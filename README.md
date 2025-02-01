## X11R6 Color names

This library contains the color names database (`rgb.txt`) provided by X11R6,
which was released in May of 1994.

Since then, the X11 color list was modified in June 2014 to add CSS level 4
colors and add entries distinguishing certain CSS from X11 colors. There have
been no other material changes.

In this library, color names are folded to lower case and the database is
provided as a sorted array.

The library was created to serve as a list of possible colors that can be
expected to be encountered in X PixMap files. X PixMap is a palettized image
format whose typical form (version 3) was mainly used in the 1990s, but
unfortunately still sticks around. Decoders and encoders for X PixMap have not
picked up the 2014 additions to the X11 color list, and should not because
allowing more color names for the format risks people using them and creating
images that are not compatible with old decoders.

Lists of colors may or may not be copyrightable, and mechanical translations of
them to a library also may or may not be copyrightable. In case they are,
`COPYING` provides the license to `rgb.txt` and to the color list in this
library. All the other content, changes, and metadata to this library are
released into the public domain and offered under `0BSD OR CC0-1.0`.
