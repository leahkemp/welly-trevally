[![DOI](https://zenodo.org/badge/253703635.svg)](https://zenodo.org/badge/latestdoi/253703635)

# welly-trevally

This welly-trevally repository contains contains all the files necessary to build this thesis into a pdf file (the actual physical thesis). Here I will give an overview of some of the important aspects of how it was coded and how to built it to a pdf.

## Build
- The R package 'bookdown' by Yihui Xie is used to knit/compile the thesis within RStudio. See: [here](https://github.com/rstudio/bookdown) and [here](https://bookdown.org/yihui/bookdown/)
- This requires the 'xelatx' latex engine and the 'natbib' citation package 

## Overall structure

- Each rmd file represents a chapter or section of the thesis
- The numbering in front of the rmd files determines the order they will appear in the final document
- There is an additional rmd file 'index.rmd' which codes for most of the thesis formatting, however, this file also calls on 'preamble.tex'

## Figures and tables
The code used to produce nearly all of the figures and tables of this thesis are included in these rmd files inline with the writing where it appears in the final thesis

- When the inline code is run, the resulting figures are exported in png or svg format to the 'images' directory
- Although I attempted to do as much of the formatting in code as possible, the finishing touches of formatting for many images and figures was undertaken manually in inkscape version 0.92.4. 
- A copy of these manually edited images were saved as an svg image file in the same 'images' directory 
- The final image to be included in the thesis was exported as a png into the 'imagesFinal' folder and integrated into the document during the thesis build
- All tables are coded for inline and are run each time the thesis is built 

## Referencing
There are two files for references

- 'endnoterefs.bib' for all references exported from endnote
- 'packages.bib' to reference the main R packages used in the thesis



