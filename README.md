# capture

> Add a button in Shiny application to take a screenshot (PNG or PDF) of a specified element. It uses [dom-to-image](https://github.com/tsayen/dom-to-image) to convert DOM elements to PNG and [jsPDF](https://github.com/MrRio/jsPDF) to generate PDF. Doesn't work in IE.

<!-- badges: start -->
[![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![R build status](https://github.com/dreamRs/capture/workflows/R-CMD-check/badge.svg)](https://github.com/dreamRs/capture/actions)
<!-- badges: end -->



## Installation

You can install the development version of {capture} from GitHub with:

```r
remotes::install_github("dreamRs/capture")
```


## Example

In UI, use `capture()`:

```r
fluidPage(

  capture::capture(
    selector = "body",
    filename = "all-page.png",
    icon("camera"), "Take screenshot of all page"
  )
  
  # ...
  
)
```


## Related packages

* [snapper](https://github.com/yonicd/snapper) : snap images of html objects in Shiny apps using `canvas2html` JavaScript
library.

