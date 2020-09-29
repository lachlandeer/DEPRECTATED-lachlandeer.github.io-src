+++
# A Demo section created with the Blank widget.
# Any elements can be added in the body: https://sourcethemes.com/academic/docs/writing-markdown-latex/
# Add more sections by duplicating this file and customizing to your requirements.

widget = "portfolio"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 60  # Order that this section will appear.

title = "Miscellaneous"
subtitle = ""

[content]
  # Page type to display. E.g. project.
  page_type = "misc"
  
  # Filter toolbar (optional).
  # Add or remove as many filters (`[[content.filter_button]]` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `[[content.filter_button]]` below.
  
  # Default filter index (e.g. 0 corresponds to the first `[[filter_button]]` instance below).
  filter_default = 0
  
  [[content.filter_button]]
    name = "Software Installation Guides"
    tag = "install-guide"
  
  [[content.filter_button]]
    name = "Reproducible Workflows"
    tag = "workflow"
  
  [[content.filter_button]]
    name = "Markdown Templates"
    tag = "md-template"

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "2"

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.

  # Background color.
  # color = "navy"
  
  # Background gradient.
  # gradient_start = "DeepSkyBlue"
  # gradient_end = "SkyBlue"
  
  # Background image.
  #image = "headers/bubbles-wide.jpg"  # Name of image in `static/img/`.
  #image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.
  #image_size = "cover"  #  Options are `cover` (default), `contain`, or `actual` size.
  #image_position = "center"  # Options include `left`, `center` (default), or `right`.
  #image_parallax = true  # Use a fun parallax-like fixed background effect? true/false

  # Text color (true=light or false=dark).
  text_color_light = false

[design.spacing]
  # Customize the section spacing. Order is top, right, bottom, left.
  padding = ["20px", "0", "20px", "0"]

[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""
+++

## Installation Guide for Software and Packages

While teaching programming skills I have assembled a set of instructions for setting up a computing environment that I find useful for economics / marketing research.

* [Detailed Installation Guide for Ubuntu / Debian Systems](https://lachlandeer.github,io/installation-guide)
    * I use this when setting up a new machine for myself. It's quite brief on details. 
* [Basic Guide for Windows, Mac and Ubuntu](https://pp4rs.github.io/installation-guide)
    * I use this when teaching. There should be a lot of details here.

## Reproducible Research Workflows

The Snakemake workflow management system helps to create reproducible and scalable data analyses. 
It was originally designed for Bioinformatics workflows, but I have found it suits research in empirical economics and marketing just as well.
Official documentation for Snakemake is [here](https://snakemake.readthedocs.io/en/stable/). 
Below are some templates that I use for my research and an extended tutorial.

* [Snakemake template for `R`](https://github.com/lachlandeer/snakemake-econ-r)
    * *Status: Under development*
    * Coauthored with [Julian Langer](https://julianlanger.github.io) (U Zurich)
    
<!---
* [Snakemake template for `Python`](https://github.com/lachlandeer/snakemake-python)
* [An extended Snakemake tutorial](https://github.com/lachlandeer/snakemake-economics)
--->

Some of my older projects use `Waf` to implement a reproducible workflow. `Waf` was introduced to me by [Hans-Martin von Gaudecker](http://wiwi.uni-bonn.de/gaudecker/index.html). 
He provides great templates [here](https://github.com/OpenSourceEconomics/econ-project-templates) in multiple programming languages along with an [extended tutorial](https://econ-project-templates.readthedocs.io/en/latest/index.html). 
It's a good alternative, but I think the Waf learning curve is a tad steeper.


## Markdown templates

Most of my written work is in markdown. Here are some templates I have used now and in the past. They may be a little outdated.

* [Article templates with `bookdown` and `rticles`](https://github.com/lachlandeer/bookdown_rticles)
* [Article template in `markdown`](https://github.com/lachlandeer/markdown-article-template)
* [Beamer slide template](https://github.com/lachlandeer/beamer-LagonBleu) with `markdown`
* [CV template](https://github.com/lachlandeer/lachlandeer-cv) with `Rmarkdown`
* [HTML slide template](https://github.com/lachlandeer/xaringan-template) with `Rmarkdown` and `xaringan`

<!---
* [UZH Thesis templates](https://github.com/lachlandeer/thesisdown-uzh) with `Rmarkdown`
* [UZH Letter template](https://github.com/lachlandeer/uzh-letter) with `Rmarkdown`
--->

<!---
## Other tutorials
Some other tutorials I have put together over the years:

* [Data Wrangling with Pandas: A Guide for Economists](https://github.com/lachlandeer/pandas-economics)
* [Estimating Econometric Models with GMM in R](https://github.com/lachlandeer/gmm-r)
--->