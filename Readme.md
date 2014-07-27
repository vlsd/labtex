To install locally on *nix systems, first determine your texmf home folder:

$ TEXMFHOME = `kpsewhich -var-value=TEXMFHOME`

And then add the sty files to it:

$ mkdir -p $TEXMFHOME/tex/latex/labtex
$ cp *.sty $TEXMFHOME/tex/latex/labtex/

In your .tex document, add

\usepackage{labtex}

after you include all other packages. Alternatively, you could just copy
the sty file you need into the same folder as the document you are
compiling.

I *think* the dependencies are only
amsmath.sty and amsfonts.sty.
