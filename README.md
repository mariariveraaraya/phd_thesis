# Understanding rumination as a form of inner speech: probing the role of motor processes

An online HTLM version of the thesis is available at https://www.barelysignificant.com/phd_thesis/ and a PDF version at https://thesiscommons.org/p6dct/.

## Abstract

Rumination is known to be a predominantly verbal process and has been proposed to be considered as such as a dysfunctional form of inner speech (i.e., the silent production of words in one's mind). On the other hand, research on the psychophysiology of inner speech revealed that the neural processes involved in overt and covert speech tend to be very similar. This is coherent with the idea that some forms of inner speech could be considered as a kind of simulation of overt speech, in the same way as imagined actions can be considered as the result of a simulation of the corresponding overt action (e.g., walking and imagined walking). In other words, the motor simulation hypothesis suggests that the speech motor system should be involved as well during inner speech production. The corollary hypothesis might be drawn, according to which the production of inner speech (and rumination) should be disrupted by a disruption of the speech motor system. We conducted a series of five studies aiming to probe the role of the speech motor system in rumination. Overall, our results highlight that although verbal rumination may be considered as a form of inner speech, it might not specifically involve the speech motor system. More precisely, we argue that rumination might be considered as a particularly strongly condensed form of inner speech that does not systematically involve fully specified articulatory features. We discuss these findings in relation to the habit-goal framework of depressive rumination and we discuss the implications of these findings for theories of inner speech production.

## Technical notes

### Premises

My dissertation is a book based on `RMarkdown` and the `bookdown` package
(<https://github.com/rstudio/bookdown>, <https://bookdown.org/>). This bookdown project was originally a fork of the demo book
(<https://github.com/rstudio/bookdown-demo>) and is largely inspired by Tristan Mahr's own dissertation: <https://github.com/tjmahr/dissertation/blob/master/README.md>. Importantly, I have used the `memoir` LaTeX class (https://ctan.org/pkg/memoir?lang=en) in combination with the `bookdown` package.

### How does it work?

The most important elements of the template are listed and discussed below:

* The `index.Rmd` file is the central file of the thesis. It contains basic metadata such as the author name, the title of the thesis, and so on (in the YAML header). Importantly, it also defines the `documenclass` (in my case, it uses the `memoir` package) and the class options. In the YAML header of this file, I also specify the bibliography files (in a better BibTeX format, issued from Zotero). The index file also contains the (English) abstract of the thesis, displayed on the welcome page of the online html version of the thesis.

* The `preamble.tex` (in the ./latex folder) file is like a usual preamble .tex file. It loads the relevant LaTeX packages, defines some commands to be used later in the thesis (such as `\initial`) and defines some formatting elements. I have tried to comment the code as much as possible but nobody's perfect.

* The `before_body.tex` (in the ./latex folder) defines elements for the cover page (specific to Univ. Grenoble Alpes). The last lines of this file may be more generally useful as they define some formatting elements for the rest of the thesis (e.g., I define the main font and set the line stretch to `\OnehalfSpacing`).

* The UGA cover page template is managed by the `cover_page.sty` style file (in the ./cover folder).

* The `_bookdown.yml` files defines the name of the outputted document (here "thesis"), the label for the chapters, the outputting directory (i.e., where outputted documents are stored) and the .Rmd files that should be included for each output format.

* Another crucial element, the `_output.yml` file defines the argument to be passed to the function creating each output. For each output format (here, gitbook, pdf, and word), it defines format-specific arguments. Importantly, for the PDF output, to be able to define a citation style (using a .csl), the `citation_package` argument should be set to `none` so that `pandoc-citeproc` is used (instead of `natbib` or `biblatex`, for instance).

* A citation style can then be applied by using the `pandoc_args` argument of the `bookdown::pdf_book` function.

Some things I have changed from previous versions of the template:

* I deactivated the default TOC from `bookdown` and defined a custom one in `00-toc.Rmd` to be able to define the order of the `00-*.Rmd` files (e.g., abstract, preface, etc).

* I deactivated the default references manager (i.e., `natbib` or `biblatex`) to be able to provide a .csl file for the references (`citation_package` in `_output.yml` needs to be `none`). See the `pandoc_args` in the `_output.yml` file.

* I have manually created a list of abbreviations in the `00-toc.Rmd` file and defined a LaTeX command to fill-in this glossary at the bottom of `preamble.tex`. I have tried to use automatic list of abbreviations such as the one in the `glossaries` package (https://www.ctan.org/pkg/glossaries) but I did not manage to make it work with `bookdown`...
