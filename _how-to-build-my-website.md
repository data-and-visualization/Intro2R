# How to Build this site:

This site is built with R Markdown's website feature.  [Read more about websites](http://rmarkdown.rstudio.com/lesson-13.html).

1. Clone from Github to RStudio

4. Manipulate files

3. `rmarkdown::render_site(encoding = 'UTF-8')`
    
5. Copy /docs web to the serving location

    - e.g. github repo served by Netlify
    - in this case:  rfun (blogdown-rfun2 on github)
    - I'm manually copying the /docs directory into the *static* directory in rfun - https://github.com/data-and-visualization/Rfun
