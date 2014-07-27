# labtex

This is a collection of LaTeX styles I've used in my grad school lab. They
might come in handy at some point.

## Installation

To install locally on *nix systems, first determine your texmf home folder
and then copy the files there:

    $ TEXMFHOME = `kpsewhich -var-value=TEXMFHOME`
    $ mkdir -p $TEXMFHOME/tex/latex/labtex
    $ cp *.sty $TEXMFHOME/tex/latex/labtex/

In your .tex document, add

    \usepackage{labtex}

after you include all other packages. Alternatively, you could just copy
the sty file you need into the same folder as the document you are
compiling.

## Dependencies

* `amsmath.sty`
* `amsfonts.sty`
* anything else I might have missed
