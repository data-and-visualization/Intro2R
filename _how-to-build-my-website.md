# How to Build this site:

This site is built with R Markdown's website feature.  [Read more about websites](http://rmarkdown.rstudio.com/lesson-13.html).

1. Clone from Github to RStudio

4. Manipulate files

3. `rmarkdown::render_site(encoding = 'UTF-8')`

    - BETTER:  Build Tab (upper-right quadrant) > Build Website
    - Can knit Rmd docs one at a time if there are problems
    - add `tango` to highlight:  `highlight: tango`
    - rename studentAssignment.Rmd to _studentAssignment.Rmd
    - exclude: ["README.md", "license.md", "intro2R.Rmd", "answers.Rmd", "*.html"]
    -     footer :: `after_body footer.html`
    - add wow-starbucks to Visualization.Rmd
    - library(datasets) ; cars <- as_tibble(rownames_to_column(mtcars, var = "makeModel"))
    - quiz students and ask if they have a preference on the dataset
    - duke.css ::      right: 50px;
    - index.Rmd  ::   add ## GIS
    - View(foo) has been turned off.  instead, make a img of clicking the environment i\pane icon
    
5. Copy /docs web to the serving location

    - e.g. github repo served by Netlify
    - in this case:  rfun (blogdown-rfun2 on github)
    - I'm manually copying the /docs directory into the *static* directory in rfun - https://github.com/data-and-visualization/Rfun
