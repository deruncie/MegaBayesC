**MegaBayesC** is an extension to **MetaLMM** that allows for BayesC priors on a set of markers affecting all traits.
    
Please treat this as a Beta version and let me know of issues running the functions.    


### Installation:
```{r}
devtools::install_github('deruncie/MegaBayesC')
```

Note: the package requires OpenMP which causes problems on a Mac. I was able to get everything to run by following these instructions: [https://mac.r-project.org/openmp/](https://mac.r-project.org/openmp/) including the addition to `~/.R/Makevars`. Installing on Unix-like machines and maybe Windows should cause fewer problems.

### Introduction:
Please see the vignette `Running_MegaLMM.Rmd` for an introduction to using **MegaLMM**

If you would like to build the vignette (see below), do:

```{r}
devtools::install_github('deruncie/MegaBayesC', build_opts = c("--no-resave-data", "--no-manual"),force = TRUE,build_vignettes = TRUE)
```

```{r}
vignette(topic = 'Running_MegaLMM',package='MegaBayesC')
```

