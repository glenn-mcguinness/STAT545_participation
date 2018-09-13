---
title: "Data Frame Exploration"
output: 
    html_document:
        theme: cerulean
        toc: true
        keep_md: true
---

## LaTeX Equations in R Markdown

Here is an equation:

$$\alpha = 5 + 2$$

Inline equation: $\alpha = 5 + 2$. 

## Data frame exploration

### Setting up

First, load the `gapminder` R package. If you don't have it installed, run `install.packages("gapminder")` in the console first.


```r
library(gapminder)
```

### What is a data frame?

It's tabular data. To get a sense of this, go ahead and print out the `gapminder` object (you might want to do this in the console!).

### Exploration of data frames

Let's explore `gapminder` with functions like `head`, `ncol`, `str`, `summary`.


```r
head(gapminder)
```

```
## # A tibble: 6 x 6
##   country     continent  year lifeExp      pop gdpPercap
##   <fct>       <fct>     <int>   <dbl>    <int>     <dbl>
## 1 Afghanistan Asia       1952    28.8  8425333      779.
## 2 Afghanistan Asia       1957    30.3  9240934      821.
## 3 Afghanistan Asia       1962    32.0 10267083      853.
## 4 Afghanistan Asia       1967    34.0 11537966      836.
## 5 Afghanistan Asia       1972    36.1 13079460      740.
## 6 Afghanistan Asia       1977    38.4 14880372      786.
```

### Extracting columns/"variables"

Let's extract a column with `$`. Maybe compute its variance.
