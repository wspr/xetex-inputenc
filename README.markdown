
THE XETEX-INPUTENC OVERRIDE PACKAGE
===================================

This package is designed to emulate LaTeX's `inputenc` package.
It's now ready for testing; I hope that it will make it into
TeX Live 2009, automatically loaded by `inputenc` itself if necessary.

Use it like the `inputenc` package:

    \usepackage[latin1]{xetex-inputenc}

The `utf8` option is default, of course, but if you're using
that then you don't need this package.


Installation
------------

Run `pdflatex` on `xetex-inputenc.dtx` to extract the `.sty` file
and produce the documentation, such as it is.


Test file
---------

The test file `xetest-latin1.tex` should then compile in all three of the
following modes:

1.   pdflatex  test-latin1
2.   xelatex   test-latin1
3.   xelatex   "\let\iffontspec\iftrue\input test-latin1"

The document requires two compilations to resolve the table of contents.
See the test file itself for more details about what each mode is testing.


_______________________
(C) Will Robertson 2009

Distributed under v1.3c or later of
the LaTeX Project Public License.

