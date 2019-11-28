# EcoDiet

*This is a work in progress!*

## R installation

EcoDiet is an R package so before anything, you should download and install/update R.

## JAGS installation

EcoDiet relies on the JAGS program to run so you will also need to download and install JAGS.

#### For Windows users

You can download JAGS from [here](https://sourceforge.net/projects/mcmc-jags/) then follow the indications.

#### For MacOS and Linux users

Try this command if you are on MacOS:
```
sudo brew update
sudo brew install jags
```

or this command if you are on Linux:
```
sudo apt-get update
sudo apt-get install jags
```

If you get an error message during installation, tou should try to follow [this post from Yu-Sung Su's blog](http://yusung.blogspot.com/2009/01/install-jags-and-rjags-in-fedora.html).

## rjags installation

You can then open R and use this command:
```
install.packages("rjags")
```

To test if everything works well, you should try this command in R:
```
library(rjags)
```
If you see the message `Linked to JAGS 4.3.0` it means everything is working fine.

## EcoDiet installation

As the EcoDiet package is only stored on GitHub for now, we need to use the `install_github` function from the `devtools` package to load it.

So we will first install and load the `devtools` package:

```{r, eval = FALSE}
install.packages("devtools")
library(devtools)
```

And now we can load the EcoDiet package:

```{r, eval = FALSE}
devtools::install_github("heloisethero/EcoDiet", auth_token='c570f1b55d68a8ae0fb38428155e19a426814d15')
```

## To learn how to use EcoDiet

The vignettes will then explain to you how to use this package. To access the vignettes you can run in R:
```
browseVignettes("EcoDiet")
```


![](man/figures/logo.PNG)