<!-- Formatting of this README was inspired by gaborcsardi's httrmock README -->



# patentsview

> An R client to the PatentsView API

[![Linux Build Status](https://travis-ci.org/crew102/patentsview.svg?branch=master)](https://travis-ci.org/crew102/patentsview)
[![Windows Build status](https://ci.appveyor.com/api/projects/status/github/crew102/patentsview?svg=true)](https://ci.appveyor.com/project/crew102/patentsview)
[![](http://www.r-pkg.org/badges/version/patentsview)](http://www.r-pkg.org/pkg/patentsview)

## Installation


```r
devtools::install_github("crew102/patentsview")
```

## Usage 

The [PatentsView API](http://www.patentsview.org/api/doc.html) provides 7 endpoints that users can query and download patent-related data from. The `patentsview` R package provides one function, `search_pv` to make it easy to interact with those endpoints. Let's take a look:



```r
library(patentsview)

search_pv(query = '{"_gte":{"patent_date":"2007-01-04"}}')
```
