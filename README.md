# Instructions

More info: http://r-pkgs.had.co.nz/vignettes.html

## Dependencies

* Pandoc: http://pandoc.org/installing.html
  ```
  # If using Homebrew
  brew install pandoc
  ```

* R Packages
  ```
  install.packages(c('devtools', 'rmarkdown', 'knitr'))
  ```

## Creating New Vignettes

1.  Add placeholder file:
    ```
    devtools::use_vignette("my-vignette")
    ```
    
2.  Edit Rmd files

3.  [Add knitr to DESCRIPTION](https://github.com/frenchja/psych/commit/fe82744a6e7abc4d2185fb2471fed631ddfa8ecd)

3.  Preview
    ```
    devtools::build_vignettes()
    ````
    
## Compiling Package with RMarkdown Vignettes

```r
# Make sure setwd() is correct set
devtools::build()
```
    
    


* More info: http://r-pkgs.had.co.nz/vignettes.html

```r
# Note that since I'm copying overview.Rnw, I'm using the same basename
devtools::use_vignette('overview')
```
