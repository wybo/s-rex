### Scan Ruby Latex

Scan Ruby Latex, s-rex in short, is a program for stitching together scanned pages and .pdfs into a single .pdf file. Requires b-rex and RMagick.

#### PNGs or other image files

To turn a series of .pngs into a .pdf

    ./s-rex my_file_0001.png

Other examples:

    s-rex my_file_0001_small.png (does not re-scale the file)

It is assumed that files are named with name_number.png

So:

    my_file_0001.png
    my_file_0002.png
    my_file_0003.png

Will be turned into

    my_file.pdf

To turn a series of .pngs into a .pdf

#### PDFs

Alternatively:

    ./s-rex My_file.CH.1.pdf

Will turn:

    My_file.CH.1.pdf
    My_file.CH.3.pdf
    My_file.CH.20.pdf

Into:

    My_file.pdf

And:

    ./s-rex *.pdf 

(list of files)

Will turn:

    01_file.pdf
    My_file3.pdf

Into:

    S-rex-out.pdf

#### Requirements

Ruby (inc rdoc, not included in Debian & Ubuntu, needs ruby and rdoc packages there), b-rex and RMagick

The program b-rex can be found here: https://github.com/wybo/b-rex

#### Copyright

Copyright (c) 2007-2016 Wybo Wiersma. Licensed under the Affero GPL: http://www.fsf.org/licensing/licenses/agpl-3.0.html
