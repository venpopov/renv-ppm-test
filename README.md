

This repo was created on the following system:

``` r
Sys.info()
```

                                                                                                    sysname 
                                                                                                   "Darwin" 
                                                                                                    release 
                                                                                                   "24.2.0" 
                                                                                                    version 
    "Darwin Kernel Version 24.2.0: Fri Dec  6 19:02:12 PST 2024; root:xnu-11215.61.5~2/RELEASE_ARM64_T6031" 
                                                                                                   nodename 
                                                                                   "Vens-MacBook-Pro.local" 
                                                                                                    machine 
                                                                                                    "arm64" 
                                                                                                      login 
                                                                                                   "vpopov" 
                                                                                                       user 
                                                                                                   "vpopov" 
                                                                                             effective_user 
                                                                                                   "vpopov" 

with a custom .Rprofile:

``` bash
cat .Rprofile
```

    source("renv/activate.R")
    if (Sys.info()["sysname"] == "Linux") {
      options(repos = c(PPM = "https://packagemanager.posit.co/cran/latest"))
      options(pkgType = "both")
    }
