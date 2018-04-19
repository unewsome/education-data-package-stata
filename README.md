# Education Data Portal - Package for Stata

Welcome to the Education Data Portal Stata Package repository. You'll need an internet connection to install and use the package.

### Install or Update the Package

If you don't have `libjson` installed, the package will automatically install it for you once you run your first `educationdata` command. Or, you can type `ssc install libjson`. The following command will install, or if the package is already installed, update the education data package.

```stata
net install educationdata, replace from("https://ui-research.github.io/education-data-package-stata/")
```

If you have trouble with this command, uninstall any existing installations using the instructions below, close and re-open Stata, then re-run the command above.

### Testing the package

First, ensure you are connected to the internet. Then run one of the simpler examples, such as:

```stata
educationdata using "college ipeds directory", sub(year=2011 fips=12)
```

### Uninstall the Package

```stata
ado uninstall educationdata
```

If you recieve the error `criterion matches more than one package` and you're running Stata 14 or newer, run the following:

```stata
adoupdate
ado uninstall educationdata
```

### Changes

To view the changes made to the package over time, see the [changelog](https://github.com/UI-Research/education-data-package-stata/blob/master/changelog.md).