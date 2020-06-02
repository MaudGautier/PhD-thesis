PhD dissertation
================

This repo contains the source code for my PhD dissertation entitled "Recombination as a driver of genome evolution: characterisation of biased gene conversion in mice". 
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
pdflatex main.tex
bibtex main.aux 
pdflatex main.tex 
pdflatex main.tex
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


