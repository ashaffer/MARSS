<style>
.nav{
    border:1px solid #ccc;
    border-width:1px 0;
    list-style:none;
    margin:0;
    padding:0;
    text-align:center;
}
.nav ul{
    margin-before: 1em;
    margin-after: 1em;
    margin-start: 0;
    margin-end: 0;
    padding:0;
}
.nav li{
    display:inline-block;
}
.nav a{
    display:inline-block;
    padding:5px;
}
</style>

<ul class="nav">
  <li><a href="#install">Install</a></li>
  <li><a href="#documentation">Documentation</a></li>
  <li><a href="#bugs">Issues</a></li>
  <li><a href="#cite">Citation</a></li>
  <li><a href="#pubs">Publications</a></li>
  <li><a href="#license">License</a></li>
  <li><a href="https://nwfsc-timeseries.github.io/MARSS/NEWS.html">NEWS</a></li>
</ul>

<img src="logot.png" align="right" style="margin:5px 0px"/>

MARSS stands for Multivariate Auto-Regressive(1) State-Space. The MARSS package is an R package for estimating the parameters of linear MARSS models with Gaussian errors.  This class of model is extremely important in the study of linear stochastic dynamical systems, and these models are important in many different fields, including economics, engineering, genetics, physics and ecology.  The model class has different names in different fields, for example in some fields they are termed dynamic linear models (DLMs) or vector autoregressive (VAR) state-space models.  The MARSS package allows you to easily fit time-varying constrained and unconstrained MARSS models with or without covariates to multivariate time-series data via maximum-likelihood using primarily an EM algorithm.

[![cran version](http://www.r-pkg.org/badges/version/MARSS)](https://cran.r-project.org/package=MARSS)
[![rstudio mirror downloads](http://cranlogs.r-pkg.org/badges/grand-total/MARSS?)](https://github.com/metacran/cranlogs.app)
[![](https://cranlogs.r-pkg.org/badges/MARSS?color=FFD700)](https://www.r-pkg.org/pkg/MARSS)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)


### INSTALL {#install}

To install MARSS from CRAN:

```
install.packages("MARSS")
library(MARSS)
```

The latest release on GitHub may be ahead of the CRAN release. To install the latest release on GitHub:
```
install.packages("devtools")
library(devtools)
install_github("nwfsc-timeseries/MARSS@*release")
library(MARSS)
```

The master branch on GitHub has work leading up to a GitHub release.  The code here may be broken though usually prelim work is done on a development branch before merging.  To install the master branch:
```
install_github("nwfsc-timeseries/MARSS")
```
If you are on a Windows machine and get an error saying 'loading failed for i386' or similar, then try
```
options(devtools.install.args = "--no-multiarch")
```
If R asks you to update packages, and then proceeds to fail at installation because of a warning that a package was built under a later R version than you have on your computer, use
```
Sys.setenv(R_REMOTES_NO_ERRORS_FROM_WARNINGS=TRUE)
```
To install an R package from GitHub, you need to be able to build an R package on your machine. If you are on Windows, that means you will need to install [Rtools](https://cran.r-project.org/bin/windows/Rtools/). On a Mac, installation should work fine; you don't need to install anything.

### DOCUMENTATION and TUTORIALS  {#documentation}

- [Quick Start Guide](https://cran.r-project.org/web/packages/MARSS/vignettes/Quick_Start.pdf).
- [User Manual](https://cran.r-project.org/web/packages/MARSS/vignettes/UserGuide.pdf) - The extensive user manual included in the package has many examples of how to fit MARSS models to a variety of data sets.
- [ATSA lab book](https://nwfsc-timeseries.github.io/atsa-labs/) - Many applications are also covered in our Applied Time Series Analysis book developed from the labs in our course.
- [ATSA course website](https://nwfsc-timeseries.github.io/atsa/) - We have lectures and all material from our course on our course website.
- [Wiki](https://nwfsc-timeseries.github.io/MARSS-wiki/) - The MARSS wiki has misc and random projects and code.


### ISSUES and BUG REPORTS {#bugs}

Issues? [https://github.com/nwfsc-timeseries/MARSS/issues]()

### CITATION  {#cite}

If you use MARSS results in publications, please cite the primary citation:

Holmes, E. E., Ward, E. J. and Wills, K. (2012) MARSS: Multivariate Autoregressive State-space Models for Analyzing Time-series Data. The R Journal. 4(1):11-19

You can also cite the package as you would other R packages:

Elizabeth Holmes, Eric Ward, Mark Scheuerell, and Kellie Wills (2018). MARSS: Multivariate Autoregressive State-Space Modeling. R package version 3.10.4.

Update the version number and year if you use a more recent version on GitHub.

### PUBLICATIONS {#pubs}

To see our publications using MARSS models, see the [Applied Time Series Analysis website](https://nwfsc-timeseries.github.io/).


### LICENSE {#license}

MARSS was developed by US federal government employees as part of their official duties. As such, it is not subject to copyright protection and is considered “public domain” (see 17 USC § 105). Public domain software can be used by anyone for any purpose, and cannot be released under a copyright license.
