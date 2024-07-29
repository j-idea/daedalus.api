
<!-- README.md is generated from README.Rmd. Please edit that file -->

# daedalus.api

<!-- badges: start -->
[![Project Status: Concept – Minimal or no implementation has been done yet, or the repository is only intended to be a limited example, demo, or proof-of-concept.](https://www.repostatus.org/badges/latest/concept.svg)](https://www.repostatus.org/#concept)
[![CRAN status](https://www.r-pkg.org/badges/version/daedalus.api)](https://CRAN.R-project.org/package=daedalus.api)
[![Codecov test coverage](https://codecov.io/gh/jameel-institute/daedalus.api/branch/main/graph/badge.svg)](https://app.codecov.io/gh/jameel-institute/daedalus.api?branch=main)
[![R-CMD-check](https://github.com/jameel-institute/daedalus.api/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/jameel-institute/daedalus.api/actions/workflows/R-CMD-check.yaml)
[![Build status](https://badge.buildkite.com/2fe5d34f1b4c4681b4e0e8d464f4fdaf44358fc48325b92580.svg)](https://buildkite.com/mrc-ide/daedalus-dot-api)
<!-- badges: end -->

_daedalus.api_ is an API package for the [_daedalus_ package](https://github.com/jameel-institute/daedalus) and is primarily intended for internal use.

## Installation

You can install the development version of daedalus.api from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("jameel-institute/daedalus.api")
```

## Quick start

```sh
# the image will be assigned the tag 'latest'
docker pull mrcide/daedalus.api:latest

# run the container
# see docker run --help for options
docker run -d --name daedalus-api --rm -p 8001:8001 mrcide/daedalus.api:latest

# check root endpoint `GET/`
curl -s http://localhost:8001 | jq

# stop the service
docker stop daedalus-api
```

## Related projects

See the [_daedalus_ package](https://github.com/jameel-institute/daedalus) which implements the DAEDALUS integrated model of economic, social, and health costs of a pandemic.
