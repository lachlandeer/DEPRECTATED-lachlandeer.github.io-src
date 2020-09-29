## README

How to Build this site manually

1. [If starting from scratch...] Clone the github repo into RStudio  

    - My preferred method of making new repos as RStuio Projects...
    
        1. Start at Github.com > New Repo
        1. Clone [new & empty] Repo as new project into Rstudio IDE running on localhost
        1. git push -- README.md, license.md, and .gitignore
    
2. `library(blogdown)` [Resources:  [github](https://github.com/rstudio/blogdown), [Yihui's Book](https://bookdown.org/yihui/blogdown/)]

    - Dependencies:
    
        - `devtools::install_github('rstudio/blogdown')`
        - `blogdown::install_hugo()`
            - only need to do this once, but...
            - might need to, occasionally but not initially, run `blogdown::update_hugo()`
        - `blogdown::new_site(theme = "gcushen/hugo-academic")` 
            - must be a completely empty directory except for .Rproj file
            - view [other theme](https://themes.gohugo.io/) options
                - See [Yihui's recommendation](https://github.com/rstudio/blogdown#blogdown) of selecting one of only a few workable themes for newbies
    
3. `blogdown::serve_site()`
4. Edit via *Rmarkdown* or *markdown* in the `content` directory and subdirs

    - Initially, you will have edited the `config.toml`, plus `layouts`, and `static` directories (e.g. CSS, templates, etc. and such)
    
5. Make customizations and stylistic (i.e. non-content) changes (CSS, see ["*static*"](https://bookdown.org/yihui/blogdown/templates.html)) in the `static` directory, where the sub-hierarchy of `static` mirrors the sub-hierarchy into `public` 

    - Do not need to mirror the entire sub-hieary.  Customize/mirror only as necessary and appropriate.
    
5. Override `layouts` by ghosting the `themes/../layouts/...` sub-hiearchy into the `layouts` directory.  See [custom-layours documentation](https://bookdown.org/yihui/blogdown/custom-layouts.html)

5. Deployment on [Github Pages](http://pages.github.com)  

    - Copy the `public` folder to `lachlandeer.github.io` (eg `cp -r public/* path/to/lachlandeer.github.io/`)
    - Ensure `lachlandeer.github.io` has an additional file `.nojekyll` (it can be be empty)
    - push from `lachlandeer.github.io`

6. Extra stuff to build? I have slides in the directory `static/slides`, if we want to pass these over to the site, run `blogdown::build_dir("static/slides/")` before copying!