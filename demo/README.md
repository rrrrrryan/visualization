# demo

https://rrryan.shinyapps.io/demo/

This code comes from [this](https://shiny.rstudio.com/articles/shinyapps.html) tutorial.


## Quick Version:
1. Copy this repo.
2. Make an account on [shinyapps.io](www.shinyapps.io).
3. Locally, install the following packages. Be sure to load `rsconnect`:
```
install.packages(c("ggplot2", "shiny", "rsconnect"))
library(rsconnect)
```
5. Go to the [tokens page](https://www.shinyapps.io/admin/#/tokens) and click show to get the following snippet automatically filled out with your own info.
```
rsconnect::setAccountInfo(name="<ACCOUNT>", token="<TOKEN>", secret="<SECRET>")
```
6. Set your working directory to this `/demo/` folder.


### Test Locally
```
library(shiny)
runApp()
```

### Deply
```
library(rsconnect)
deployApp()
```

This will deploy to **`https://username.shinyapps.io/folder/`**, where `folder` is the name of the folder containing `server.R` and `ui.R`.
