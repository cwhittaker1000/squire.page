
<!-- README.md is generated from README.Rmd. Please edit that file -->

# squire.page.sarsX

<!-- badges: start -->
<!-- badges: end -->

This package stores miscellaneous R functions used in the repo
[global-lmic-reports](https://github.com/mrc-ide/global-lmic-reports-orderly)
and other repos that use [nimue](https://github.com/mrc-ide/nimue) fits.
The thinking behind storing these as an external package means that they
can be kept consistent across multiple repos and
[orderly](https://github.com/vimc/orderly) tasks. The majority of
functions are variations on the fitting functions in
[squire](https://github.com/mrc-ide/squire). These are not added to the
base squire or nimue packages as they are too specific in their usage.

Named after the position typically held before a becoming a squire.

## Contents

Please see the [GitHub page](https://mrc-ide.github.io/squire.page/) for
more information.

Likelihood and MCMC functions for the excess mortality fitting. These
account for fitting to weekly data and not daily, and also allow for
poisson instead of negative binomial fitting.

Likelihood functions for the LMIC-reports. These allow fitting to cases
at the tail of the epidemic and time varying hospitalisation modifiers
(should be added to squire at some point).

Functions to simulate draws from model output given different numbers of
vaccines. Also a similar function from the LMICs (should simplify this).

Functions for setting up future scenarios in the LMIC projections.

A different method for fitting any squire/nimue model by adjusting Rt
values over short periods of time.

Various functions for plotting R and deaths over time, should be
compatible with any version of the fits.

## Installation

This package depends on both [nimue](https://github.com/mrc-ide/nimue)
and [squire](https://github.com/mrc-ide/squire). You can install
squire.page like so:

``` r
#devtools::install_github("mrc-ide/squire")
#devtools::install_github("mrc-ide/nimue")
devtools::install_github("mrc-ide/squire.page")
```

## To Do:

-   Ensure all functions are documented
