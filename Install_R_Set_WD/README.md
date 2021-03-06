
## Instructions to Install R 

The best and quickest way to start working is installing `R-Studio`. Below are some quick steps to install R-studio in Ubuntu 18.04

1. In order to install RStudio on Ubuntu 18.04 we will first need to install the r-base package. Open up terminal and enter: 
```
$ sudo apt update
$ sudo apt -y install r-base
```

2. Download the latest Ubuntu/Debian RStudio `*.deb` package available from [R Studio Download](https://rstudio.com/products/rstudio/download/#download)

3. The easiest way to install DEB file on Ubuntu Linux is by using the gdebi command. In case gdebi is not available on your system you can install it by executing the bellow command: 

```
$ sudo apt install gdebi-core
```

4. Install the downloaded package
```
$ sudo gdebi rstudio-1.2.5033-amd64.deb
```

5. run the below command to start r studio
```
rstudio
```


## Instructions to setup a working directory and write your first R file.

1. Create a directory with name `R-Experiments` on you Desktop.
2. Open R-studio and type the below command in the console to see your current WD.
```
> getwd()
```
3. Type the below command to set the working directory.
```
> setwd("~/Desktop/R-Experiments")
```
4. Create a new file, name it with `first.R` , enter the below code and save it.
```
> myfunc <- function(x){
    y <- rnorm(x)
    mean(y)
}
```
5. Load the above function into the console and run the fucntion
```
> source('first.R')
>ls()
myfunc
> myfunc(100)
[1] 0.02964244
```
