# Notes to fix data loading

- Data loading should do two things

    1. `foo <- read_csv("foo.csv")`
    2. Then operate on the mtcars transformed into a tibble
    
        - `library(datasets)`
        - `cars <- as_tibble(rownames_to_column(mtcars, var = "makeModel"))`
        
