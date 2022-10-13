---
abstract: " "
title: bioCancer- A Shiny App to visualize and analyse interactively Multi-Assays of Cancer Genomic Data.
summary: bioCancer is a browser-based interface for Cancer Genomics Data analysis and visualization developped by R, and based on the Shiny package.
author_notes:
- Equal contribution
authors:
- admin
date: "2016-09-01T00:00:00Z"
doi: "10.18129/B9.bioc.bioCancer"
featured: false
image:
  caption:
  focal_point: ""
  preview_only: false
projects: []
publication: ''
publication_short: ""
publication_types:
- "2"
publishDate: "2016-09-01T00:00:00Z"
url_code: "https://github.com/kmezhoud/bioCancer"
url_dataset: ""
url_pdf: "https://www.bioconductor.org/packages/release/bioc/manuals/bioCancer/man/bioCancer.pdf"
url_poster: ""
url_project: "https://www.bioconductor.org/packages/release/bioc/vignettes/bioCancer/inst/doc/bioCancer.html"
url_slides: ""
url_source: ""
url_video: ""
---

# bioCancer - Interactive Multi-OMICS Cancers Data Visualization and Analysis
[![releaseVersion](https://img.shields.io/badge/release%20version-1.6.00-green.svg?style=flat)](https://bioconductor.org/packages/bioCancer)[![develVersion](https://img.shields.io/badge/devel%20version-1.7.04-green.svg?style=flat)](https://github.com/bioCancer)[![Bioc](https://www.bioconductor.org/shields/years-in-bioc/bioCancer.svg)](https://www.bioconductor.org/packages/devel/bioc/html/bioCancer.html#since)[![total](https://img.shields.io/badge/downloads-1759/total-blue.svg?style=flat)](https://bioconductor.org/packages/stats/bioc/bioCancer)
[![rank](https://img.shields.io/badge/rank%20/total-blue.svg?style=flat)](https://bioconductor.org/packages/stats/bioc/bioCancer)
<!--[![Coverage Status](https://img.shields.io/coveralls/kmezhoud/bioCancer.svg)](https://coveralls.io/r/kmezhoud/bioCancer?branch=master) -->
`r badge_bioc_download("bioCancer, "total", "blue", "total")`

https://cranlogs.r-pkg.org/badges/stringr

[bioCancer](
https://kmezhoud.github.io/bioCancer/
) is a browser-based interface for Cancer Genomics Data analysis and visualization developped by [R](https://www.r-project.org/), and based on the [Shiny](https://www.rstudio.com/shiny/) package.

#### Interactivities

bioCancer is listening user setting. Results are updated immediately when inputs are changed (i.e., no separate dialog boxes).

#### Context

bioCancer focuses on Cancer Genomics data visualisation and Genes Classifications.

## Circomics: Pull User genetic profiles with existing Cancer studies

<img src="Circomics_demo.gif">
<!--
It is inspired from [radiant](https://github.com/vnijs/radiant) developed by <a href="https://rady.ucsd.edu/faculty/directory/nijs/" target="\_blank">Dr. Vincent Nijs</a>. 
-->

## Preprocessing and Plotting

<img src="S3Video2.gif">


## Genes Classification and Biological terms Clustering

<img src="S4Video3.gif">


## Network modeling example
<!--
![Network modeling](./inst/extradata/imgs/demoReactome.gif)
-->
<img src="S5Video4.gif">

<!--
## Key features

- Explore: Quickly and easily summarize, visualize, and analyze your data
- Cross-platform: It runs in a browser on Windows, Mac, and Linux
- Reproducible: Recreate results and share work with others as a state file or an [Rmarkdown](https://rmarkdown.rstudio.com/) report
- Programming: Integrate bioCancer's analysis functions into your own R-code
- Context: Data and examples focus on business applications

<iframe width="640" height="375" src="https://www.youtube.com/embed/ioHopyfD2f0" frameborder="0" allowfullscreen></iframe>
-->

<!--
#### Reproducible

Simply saving output is not enough. You need the ability to recreate results for the same data and/or when new data become available. Moreover, others may want to review your analysis and results. Save and load the state of the application to continue your work at a later time or on another computer. Share state files with others and create reproducible reports using [Rmarkdown](https://rmarkdown.rstudio.com/). See also the section on `Saving and loading state` below
-->

<!--
#### Programming

Although bioCancer's web-interface can Processing quite a few data and analysis tasks, at times you may prefer to write your own code. bioCancer provides a bridge to programming in R(studio) by exporting the functions used for analysis. For more information about programming, see Radiant [programming](https://vnijs.github.io/radiant/programming.html) page on the documentation site.
-->



## How to install bioCancer


- Required: [R](https://cran.rstudio.com/) version 3.2 or later
- Required: A modern browser (e.g., [Chrome](https://www.google.com/intl/en/chrome/browser/desktop/) or Safari). Internet Explorer (version 11 or higher) should work as well
- Recommended: [Rstudio](https://www.rstudio.com/products/rstudio/download/)

bioCancer courant release:
```r
 source("https://bioconductor.org/biocLite.R")
 biocLite("bioCancer")
```

bioCancer is under development:
```r
 devtools::install_github("kmezhoud/bioCancer")
 library("bioCancer")
```


When bioCancer starts you will see a table of available Cancer Studies.  To close the application click on `Quit` in the Navigation bar and then click the `Quit` button on the left of the screen. The bioCancer process will stop and the browser window will close (or gray-out).



## Documentation


Documentation and tutorials are available in the bioCancer web interface (the `?` icons and the `Help` menu).

<!--
## Saving and loading state from bioCancer
To save your analyses save the state of the app to a file by clicking on the <i title='Save' class='fa fa-save'></i> icon in the navbar and then on `Save state` (see also the `Data > Processing > Manage` tab). You can open this state file at a later time or on another computer to continue where you left off. You can also share the file with others that may want to replicate your analyses. As an example, load the state_file [`example.rda`](https://github.com/vnijs/radiant/blob/master/inst/examples/RadiantState.rda?raw=true) through the Data > Manage tab. Go to `Processing > View`, `Processing > Visualize` to see some of the settings. There is also a report in `R > Report` that was created using the bioCancer interface. The html file [`ExampleState.html`](https://github.com/vnijs/radiant/blob/master/inst/examples/RadiantState.html?raw=true) contains the output.


Loading and saving state also works with Rstudio. If you start bioCancer from Rstudio and use <i title='Power off' class='fa fa-power-off'></i> > `Stop` to stop the app, lists called `r_data` and `r_state` will be put into Rstudio's global workspace. If you start bioCancer again using `bioCancer()` it will use these lists to restore state. This can be convenient if you want to make changes to a data file in Rstudio and load it back into bioCancer. Also, if you load a state file directly into Rstudio it will be used when you start bioCancer to recreate a previous state.

```r
numericInput("sm_comp_value", "Comparison value:", state_init('sm_comp_value',sm_args$comp_value))
```
-->
## Acknowledgment


bioCancer is a collaborative work . Processing panel is adapted from [radiant](https://github.com/vnijs/radiant). I would like to thank <a href="https://rady.ucsd.edu/faculty/directory/nijs/" target="\_blank"> Dr. Vincent Nijs</a> for sharing his work for R community.

<!--
## License

bioCancer is licensed under the <a href="https://www.tldrlegal.com/l/AGPL3" target="\_blank">AGPLv3</a>. The documentation and videos on this site and the bioCancer help files are licensed under the creative commons attribution, non-commercial, share-alike license <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/" target="_blank">CC-NC-SA</a>.

As a summary, the AGPLv3 license requires, attribution, including copyright and license information in copies of the software, stating changes if the code is modified, and disclosure of all source code.

-->
