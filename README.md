# plautopatch

Japanese pLaTeX/upLaTeX formats and packages often conflict
with other LaTeX packages which are unaware of pLaTeX/upLaTeX.
In the worst case, such packages throw a fatal error or
end up with a wrong output.

The goal of this package "plautopatch" is that
there should be no need to worry about such incompatibilities,
because specific patches are loaded automatically
whenever necessary.
This helps not only to simplify source files, but also
to make the appearance of working pLaTeX/upLaTeX sources
similar to those of ordinary LaTeX ones.

The following patches are currently registered:

- doc (latex) -> pldocverb (maintained here!)
- tracefnt (latex) -> ptrace/uptrace (platex/uplatex)
- fltrace (latex) -> pfltrace (platex)
- array (latex-tools) -> plarray (platex-tools)
- array (latex-tools) + plext (platex) -> plextarray (platex-tools)
- delarray (latex-tools) + plext (platex) -> plextdelarray (platex-tools)
- colortbl + plext (platex) -> plextcolortbl (maintained here!)
- arydshln -> plarydshln (maintained here!)
- arydshln + plext (platex) -> plextarydshln (maintained here!)
- siunitx -> plsiunitx (maintained here!)
- collcell -> plcollcell (maintained here!)
- everysel (ms) -> pxeverysel (platex-tools)
- everyshi (ms) -> pxeveryshi (platex-tools)
- atbegshi (oberdiek) -> pxatbegshi (platex-tools)
- ftnright (latex-tools) -> pxftnright (platex-tools)
- multicol (latex-tools) -> pxmulticol (platex-tools)
- xspace (latex-tools) -> pxxspace (platex-tools)
- textpos -> pxtextpos (maintained here!)
- pdfpages -> pxpdfpages (maintained here!)
- stfloats (sttools) -> pxstfloats (pxsttools)
- hyperref -> pxjahyper (by Takayuki YATO)
- pgfrcs (pgf) -> pxpgfrcs (maintained here!)
- pgfcore (pgf) -> pxpgfmark (by Takayuki YATO)

## Requirements

This package depends on "filehook" package,
written by Martin Scharrer.

## Miscellaneous

This bundle may distribute some tiny patches
together with the main package.
All packages are meant for use with pLaTeX/upLaTeX.
Short information:

- pldocverb.sty:
    Patch for doc.sty (latex) to improve
    compatibility with `\verb` redefinition in pLaTeX.
- plextcolortbl.sty:
    Patch for colortbl.sty (by David Carlisle) to improve
    compatibility with plext.sty in pLaTeX.
- plarydshln.sty:
    Patch for arydshln.sty (by Hiroshi Nakashima) to improve
    compatibility with pLaTeX kernel.
- plextarydshln.sty:
    Patch for arydshln.sty (by Hiroshi Nakashima) to improve
    compatibility with plext.sty in pLaTeX.
- plsiunitx.sty:
    Patch for siunitx.sty (by Joseph Wright) to fix
    conflict with plarray.sty (platex-tools).
- plcollcell.sty:
    Patch for collcell.sty (by Martin Scharrer) to fix
    conflict with plarray.sty (platex-tools).
- pxtextpos.sty:
    Patch for textpos.sty (by Norman Gray) to support
    Japanese-style crop marks (called 'tombow' in Japanese).
- pxpdfpages.sty:
    Patch for pdfpages.sty (by Andreas Matthias) to support
    Japanese-style crop marks (called 'tombow' in Japanese).
- pxpgfrcs.sty:
    Patch for pgfrcs.sty (part of PGF) to support
    Japanese classes for vertical writing.
- pxstfloats.sty:
    Patch for stfloats.sty (sttools) to improve
    compatibility with pLaTeX kernel.
    Actually part of pxsttols (https://github.com/aminophen/pxsttools)
    but included here for convenience.

## Installation

- *.sty -> $TEXMF/tex/platex/plautopatch
- *.tex, *.pdf -> $TEXMF/doc/platex/plautopatch

## Repository

The bundle is maintained on GitHub:
  https://github.com/aminophen/plautopatch

## License

The bundle may be distributed and/or modified under the terms of
the 3-clause BSD license (see [LICENSE](./LICENSE)).

## Release Date

$RELEASEDATE

Hironobu Yamashita
