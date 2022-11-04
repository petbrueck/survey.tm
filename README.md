
# r2.tms

<!-- badges: start -->
<!-- badges: end -->

Collection of wrappers for Translation Management for surveys/censuses.
TBC.

## Installation

You can install the development version of r2.tms through

``` r
devtools::install_github("petbrueck/r2.tms")
```

## Usage

### Set up

Before working with one or more questionnaires, you need to get a Google
Worksheet that will server as the “Translation Master Sheet”.

To this end

``` r
#Optional: Indicate to `googlesheets4` which mail you will use. Avoids selecting pre-authorised account manually. 
googlesheets4::gs4_auth(email = "your.email@address.com")
#Set up sheet
setup_tsheet(
    name.ssheet="Project X: Translation Sheet",
    translation.languages=c("German","French")
)
```
