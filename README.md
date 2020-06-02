PhD thesis
==========

This repo contains the source code for my PhD dissertation entitled *Recombination as a driver of genome evolution: characterisation of biased gene conversion in mice*. 
The final work is available [online](https://tel.archives-ouvertes.fr/tel-02435079) (and [here](https://tel.archives-ouvertes.fr/tel-02435079/document) is the direct access to the resulting .pdf file).




## Usage

To get the resulting main.pdf file from the source code provided in this repo, do the following steps.

First, clone the repository:
```
git clone https://github.com/MaudGautier/PhD-dissertation.git
```

Second, download the figures from [this link](https://drive.google.com/file/d/1IZKU3mR3yS3XeDWsDx0acAj7uOKOXZWc/view?usp=sharing).
Unzip the file and put the `figures` folder in the root directory of the cloned repository.


Third, run the following command lines to get the final .pdf file:
```
pdflatex main.tex # Create main.aux (from \cite{...} arguments)
bibtex main.aux   # Create main.bbl (from .bib files and main.aux)
pdflatex main.tex # Include .bbl items in bibliography 
pdflatex main.tex # Include correct labels to \cite{...} arguments in main.pdf
pdflatex main.tex # Add citation page number within references
```

Note that it is necessary to run `pdflatex` three times to have the correct final result (for a more detailed explanation, read [this page](https://tex.stackexchange.com/questions/53235/why-does-latex-bibtex-need-three-passes-to-clear-up-all-warnings)).




## Credits

This work uses the OxThesis LaTeX template, published in 2015 on [the Oxford Echoes blog](https://www.oxfordechoes.com/oxford-thesis-template/) by John McManigle.
This template is based on a [template by Keith Gillow](https://www.maths.ox.ac.uk/members/it/faqs/latex/thesis-class) dating from 1997, which was [adapted in 2007 by Sam Evans](http://evansresearch.org/2010/05/oxford-thesis-latex-template/).
I then modified it to get the result available in this repo.




## Citation

If you use any of the content of this work, please cite:

> Gautier, M. (2019). *Recombination as a driver of genome evolution: characterisation of biased gene conversion in mice.* PhD thesis, Universit\'e Claude Bernard - Lyon I.

You are free to use the template and make it your own!



## Versions of pdflatex and bibtex

Information on the version of pdflatex used (`pdflatex --version`):
```
pdfTeX 3.14159265-2.6-1.40.17 (TeX Live 2016)
kpathsea version 6.2.2
Copyright 2016 Han The Thanh (pdfTeX) et al.
There is NO warranty.  Redistribution of this software is
covered by the terms of both the pdfTeX copyright and
the Lesser GNU General Public License.
For more information about these matters, see the file
named COPYING and the pdfTeX source.
Primary author of pdfTeX: Han The Thanh (pdfTeX) et al.
Compiled with libpng 1.6.21; using libpng 1.6.21
Compiled with zlib 1.2.8; using zlib 1.2.8
Compiled with xpdf version 3.04
```

Information on the version of bibtex used (`bibtex --version`)
```
BibTeX 0.99d (TeX Live 2016)
kpathsea version 6.2.2
Copyright 2016 Oren Patashnik.
There is NO warranty.  Redistribution of this software is
covered by the terms of both the BibTeX copyright and
the Lesser GNU General Public License.
For more information about these matters, see the file
named COPYING and the BibTeX source.
Primary author of BibTeX: Oren Patashnik.
```

